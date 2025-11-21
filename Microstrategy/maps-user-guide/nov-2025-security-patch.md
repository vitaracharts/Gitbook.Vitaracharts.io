---
description: Security patch for potentiall SSRF vulnerability
---

# Nov 2025 Security Patch

### VitaraMaps SSRF Security Patch Drop-IN –Deployment Instructions



Download URL: [https://vchost.vitaracharts.com/distributions/Maps/5.3.6.175/dropIn/VitaraMaps.zip](https://vchost.vitaracharts.com/distributions/Maps/5.3.6.175/dropIn/VitaraMaps.zip)

[https://vchost.vitaracharts.com/distributions/Maps/5.3.6.175/dropIn/VitaraMapsLibrary.zip](https://vchost.vitaracharts.com/distributions/Maps/5.3.6.175/dropIn/VitaraMapsLibrary.zip)



This patch provides the updated security-hardened versions of\
fileLoader.jsp, fileLoader.aspx.\
It is designed as a drop-in replacement for VitaraMaps versions 5.3.1 through 5.3.6.

Follow the steps below to deploy the patch in all required MicroStrategy components.

***

#### 1. Contents of the Patch

The patch package contains:

**VitaraMaps**/

&#x20;   fileLoader.jsp

&#x20;   fileLoader.aspx



**VitaraMapsLibrary**/

&#x20;   fileLoader.jsp

&#x20;   fileLoader.aspx

These files must overwrite the existing versions of the files in the VitaraMaps and VitaraMapsLibrary installation.

***

#### 2. Where to Apply the Patch

The patch must be applied in all environments where VitaraMaps are used:

1. MicroStrategy Web

\<WebRoot>/plugins/VitaraMaps/

2. MicroStrategy Library

\<LibraryRoot>/plugins/VitaraMapsLibrary/

3. PDF Export Engine (Export Server)

\<PDFExportRoot>/plugins/VitaraMaps/

Each of these components maintains its own plugins folder, so all relevant locations should be updated.

***

#### 3. Deployment Steps

**Step 1 — Extract the Patch**

Download and unzip:

* VitaraMaps.zip
* VitaraMapsLibrary.zip (Library distribution only)

You will see directories:

VitaraMaps/

VitaraMapsLibrary/     (for Library only)

containing the updated fileLoader files.

***

#### Step 2 — Copy Over Existing Installation

Navigate to each MicroStrategy component’s VitaraMaps folder, for example:

\<WebRoot>/plugins/VitaraMaps/

\<LibraryRoot>/plugins/VitaraMapsLibrary/

\<PDFExportResources>/plugins/VitaraMaps/

Then:

* Copy the extracted VitaraMaps (or VitaraMapsLibrary) folder on top of the existing folder (i.e. into the \~/plugins/ folder). Alternatively you can choose to overwrite each file individually\
  When prompted, choose Replace / Overwrite all files.
* This ensures the old fileLoader logic is replaced with the secure version.

***

#### Step 3 — Restart the Web Server

After replacing the files, restart services:

* Tomcat / IIS / Web Server (for MicroStrategy Web and MicroStrategy Library)
* PDF Export Engine

This ensures the updated fileLoader code is picked up.

***

#### Step 4 Verification - How to Confirm Patch is Working

To verify that the SSRF protection is active, you can test the behavior of fileLoader.jsp (or fileLoader.aspx) directly using a harmless public URL such as [https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/sample.txt](https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/sample.txt).

**Test AFTER adding the Patch**

Open the following URL in the browser:

For: MicroStrategy Web

https://\<YourServer>:\<port>/MicroStrategy/plugins/VitaraMaps/fileLoader.jsp?file=https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/sample.txt

For: MicroStrategy Library

https://\<YourServer>:\<port>/MicroStrategy/plugins/VitaraMapsLibrary/fileLoader.jsp?file=https://vchost.vitaracharts.com/distributions/5.3.9.215/dropIn/sample.txt

#### Expected Result With Fix (Patch Working)

You should see a JSON response similar to:

null({status:400, msg:'**host not allowed**', data:'bnVsbA==', type:'null', ctx:'null'})

This means the patch is correctly blocking external URLs.

***

**If instead the following result is seen then you’re still using the old file.**

**Result Without Fix**:

null({status:200, msg:'**success**', data:'WW91IGhhdmUgbG9hZGVkIGFuIGV4dGVybmFsIHJlc291cmNlIGZyb20gVml0YXJh', type:'null', ctx:'null'})

***

\
\
<br>
