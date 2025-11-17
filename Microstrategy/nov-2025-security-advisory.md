# Nov 2025 Security Advisory

## Server-Side Request Forgery (SSRF) Vulnerability in File Loader Endpoints

Nov 2025

***

### 1. Vulnerability Description

A Server-Side Request Forgery (SSRF) vulnerability was identified in the fileLoader.jsp and fileLoader.aspx endpoints used by VitaraCharts and VitaraMaps.

These endpoints accept a file parameter, which was originally intended to load external SVG, JPEG and PNG files. However, the parameter did not sufficiently validate the requested URL or block dangerous network paths.

#### Impact:

Please note that the file loader is only accessible to users who have access to the MicroStrategy web server; i.e if it is deployed for access only within the enterprise intranet, then only the intranet users will be able to access the file.

If unaddressed, this issue could allow unintended access to certain internal or protected network endpoints through the server. In some cases, this might include retrieving information from internal services, cloud metadata APIs, or probing network ports. While the severity depends on each customer’s internal environment and configurations, the vulnerability could potentially allow an attacker to use the server to relay requests to locations that should not normally be accessible.

This aligns with the attack vector publicly described in CVE-2025-57305.

***

### 2. Fixes Implemented to Mitigate the Vulnerability

We implemented a multi-layered SSRF defense system across both JSP and ASPX versions of the endpoint.\
Each layer independently blocks malicious requests.\
The patch release with the fixes is expected to be made generally available by the 27th of November 2025

#### 2.1 Strict Protocol Restrictions

Only HTTP and HTTPS URLs are allowed; all other protocols are blocked.

#### 2.2 External Domain Allowlist

A new /custom/whitelist.txt file controls which domains can be accessed. Only domains listed there are permitted.

#### 2.3 Private/Internal IP Blocking

All internal and localhost IP ranges (IPv4 and IPv6) are automatically blocked.

#### 2.4 DNS Rebinding Protection

The server checks that all resolved IPs are public and not internal.

#### 2.5 Socket-Level IP Validation

A secondary connection check ensures the actual destination IP is also public, preventing DNS tricks.

#### 2.6 Port Restrictions

Only standard web ports (80 and 443) are allowed.

#### 2.7 Response Size Limit

Remote responses are capped at 3 MB to prevent performance issues.

#### 2.8 Redirect Blocking

HTTP redirects are disabled to avoid indirect access to internal systems.

***

### 3. Customer Action Required

Once the new patch is installed, customers must:

#### 1. Provide Approved Whitelisted Domains

update the file:

* \~/plugins/VitaraCharts/custom/whitelist.txt

This file controls which external URLs VitaraCharts is allowed to load.

Add each allowed domain on its own line. Examples:

* svgrepo.com
* cloud.vitaracharts.com
* yourcompanycdn.com

2\. Review External Resources in Your Dashboards

If your dashboards reference external SVG markers, background-images please ensure their hostnames are included in the whitelist file.

#### 3. Update Older or Unsupported URLs

If your dashboards previously used:

* internal server URLs
* non-HTTPS URLs
* IP addresses

**IMPORTANT** : These will now be blocked. Please update them to use safe, whitelisted domain names.

#### 4. Firewall Considerations

If your environment restricts outbound traffic, ensure that MicroStrategy is allowed to reach the domains added to the whitelist.

Only explicitly allowed, public, safe domains can be accessed.

\
