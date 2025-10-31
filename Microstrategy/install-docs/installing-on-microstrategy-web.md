# Installing VitaraCharts on MicroStrategy Web

### 1. Download

1. Download the web version of VitaraCharts from the official download site.\
   (Refer to the [Main page](https://www.vitaracharts.com/ms-product-downloads) for the latest links.)\
   ![](<../.gitbook/assets/unknown (15).png>)

### 2. New Installation

Follow the steps below if this is your first time installing VitaraCharts :

1. **Download and Extract**\


* Download the VitaraCharts.zip file.
* Unzip it to extract the VitaraCharts folder.

&#x20;2\. **Stop the Web Server**

* Stop IIS, Tomcat, or the equivalent web server.

**3. Remove Existing Installation**

* Delete any existing VitaraCharts folder under the plugins directory, if present.
* Do not keep backup copies of VitaraCharts inside the plugins directory.

**4. Copy the New Version**

* Copy the extracted VitaraCharts folder into the plugins directory of your MicroStrategy Web installation.
* **path**: \tomcat\webapps\MicroStrategy\plugins

**5. Verify Folder Structure**

* Ensure that the folder structure appears correctly after installation.

![](<../.gitbook/assets/unknown (16).png>)

**6. Validate Version Folders**

* Confirm that only one version folder of VitaraCharts exists within both the style and source directories:

**Tomcat/webapps/MicroStrategy/plugins/VitaraCharts/style            Tomcat/webapps/MicroStrategy/plugins/VitaraCharts/javascript/mojo/js/source**

* If multiple version folders are found, delete the entire VitaraCharts folder and redeploy the build.

**7. Apply License**

* Replace the license.txt file in the VitaraCharts folder with the license file provided to you.

**8. Restart the Web Server**

* Start IIS, Tomcat, or your equivalent web service.

**9. Clear Browser Cache**

Clear browser caches and open dossiers/documents in a new incognito window to avoid issues from previously cached license files.

## Upgrading an Existing Installation

If you already have VitaraCharts installed and are upgrading to a newer version, follow these steps carefully.

#### Step 1: Backup Customizations

Before proceeding, take a backup of the following customization files:

* **global.txt** — defines custom color palettes, fonts, etc.
* **customStyles.css** — contains individual chart style customizations.

**File locations:**

/webapps/MicroStrategy/plugins/VitaraCharts/custom/global.txt

/webapps/MicroStrategy/plugins/VitaraCharts/custom/customStyles.css

⚠️ Ensure that the **plugins** directory contains only one **VitaraCharts** folder.\
Do not keep any backup copies inside this directory.

### Step 2: Upgrade Procedure

1. **Download** the latest web version of VitaraCharts.
2. **Extract** the VitaraCharts folder from the ZIP file.
3. **Stop** the Web Server (IIS, Tomcat, or equivalent).
4. **Delete** the existing VitaraCharts folder under the plugins directory.
5. **Copy** the new VitaraCharts folder into the same location.
6. **Replace** the license.txt file with the new one provided.

**Restore** your backed-up **global.txt** and **customStyles.css** files to:

**/webapps/MicroStrategy/plugins/VitaraCharts/custom/**

7. **Start** the Web Server.
8. **Clear browser cache** and open dossiers/documents in a new browser window.

#### **Important : Set up info for the MicroStrategy export server**

If you are using the new export engine on MicroStrategy (available starting 2019 update 2) you have the option of deploying VitaraCharts locally on the export server. The procedure is detailed here [Export engine set up](https://community.microstrategy.com/s/article/New-Customization-Property-for-the-Export-Engine-Service?language=en_US)

Use this web version of VitaraCharts to copy them to the resources folder on the export server. Please do not use the library or mobile version.

#### **Note:** Starting with version 5.3.6, a new utility named Health Tool has been introduced.

This tool provides a centralized interface to verify the correct deployment of the Vitara Charts plugin and helps identify potential configuration or compatibility issues.

👉[ Click here ](health-tool.md)to access the **Health Tool**.
