---
description: Security patch release for SSRF vulnerability
---

# Nov 2025 Security Patch

### VitaraCharts SSRF Security Patch Drop-IN – Deployment Instructions

Please note that this patch needs to be and can be applied over all supported VitaraCharts versions; Currently all versions starting from 5.3.2 are supported.

Download the patch zip file from here: [https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/VitaraCharts.zip](https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/VitaraCharts.zip)

This patch provides the updated security-hardened versions of\
fileLoader.jsp, fileLoader.aspx.\
It is designed as a drop-in replacement for VitaraCharts versions 5.3.2 through 5.3.8.

Follow the steps below to deploy the patch in all required MicroStrategy components.

***

### 1. Contents of the Patch

The patch package (VitaraCharts.zip) contains:

VitaraCharts/

&#x20;   fileLoader.jsp

&#x20;   fileLoader.aspx

These files must overwrite the existing versions of the files in the VitaraCharts installation.

***

### 2. Where to Apply the Patch

The patch must be applied in all environments where VitaraCharts are used:

1. MicroStrategy Web
2. MicroStrategy Library
3. PDF Export Engine (Export Server)

Each of these components has its own plugins/VitaraCharts folder.

***

### 3. Deployment Steps

**Step 1 — Extract the Patch**

Unzip the VitaraCharts.zip file onto your local machine.

You will see a VitaraCharts directory containing the updated files.

***

**Step 2 — Copy Over Existing Installation**

Navigate to each MicroStrategy component’s VitaraCharts folder, for example:

\<WebRoot>/plugins/VitaraCharts/

\<LibraryRoot>/plugins/VitaraCharts/

\<PDFExportResources>/plugins/VitaraCharts/

Then:

* Copy the extracted VitaraCharts folder on top of the existing folder (i.e. into the \~/plugins/ folder). Alternatively you can choose to overwrite each file individually\
  When prompted, choose Replace / Overwrite all files.
* This ensures the old fileLoader logic is replaced with the secure version.

***

**Step 3 — Restart the Web Server**

After replacing the files, restart services:

* Tomcat / IIS / Web Server (for MicroStrategy Web and MicroStrategy Library)
* PDF Export Engine

This ensures the updated fileLoader code is picked up.

***

**Step 4 Verification - How to Confirm Patch is Working**

To verify that the SSRF protection is active, you can test the behavior of fileLoader.jsp (or fileLoader.aspx) directly&#x20;

Open the following URL in the browser with your  server **name/ip** and **port**; also replace the path to '**MicroStrategy**' app if needed:

https://<mark style="color:$info;">\<YourServer>:\<port>/MicroStrategy</mark>/plugins/VitaraCharts/fileLoader.jsp?file=https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/sample.txt

#### Expected Result With Fix (Patch Working)

You should see the a response similar to with the message "host not allowed" in it:

null({status:400, msg:'**host not allowed**', data:'bnVsbA==', type:'null', ctx:'null'})

This means the patch is correctly blocking external URLs.

—----------------------------------------------------------------------------------------------------------

**If instead the following result is seen then you’re still using the old file.**

Result **Without** Fix:

null({status:200, msg:'**success**', data:'WW91IGhhdmUgbG9hZGVkIGFuIGV4dGVybmFsIHJlc291cmNlIGZyb20gVml0YXJh', type:'null', ctx:'null'})

***

\
\
\
