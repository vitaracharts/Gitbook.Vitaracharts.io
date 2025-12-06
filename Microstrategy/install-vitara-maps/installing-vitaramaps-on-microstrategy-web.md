# Installing VitaraMaps on MicroStrategy Web

Overview of the VitaraMaps installation process for MicroStrategy Web environments.

#### Download

* Download the web version of VitaraMaps from the official download page.
* &#x20;You can find the latest version links on the VitaraMaps [ Main page](https://www.vitaracharts.com/ms-product-downloads).

![](<../.gitbook/assets/unknown (1) (1).png>)

### New Installation

Follow the steps below if this is your first time installing VitaraMaps:

1. **Download and Extract**

* Download the VitaraMaps.zip file.
* Unzip it to extract the VitaraMaps folder.

2. **Stop the Web Server**

* Stop IIS, Tomcat, or the equivalent web server.

3\. **Remove Existing Installation**

* Delete any existing VitaraMaps folder under the plugins directory, if present.
* Do not keep backup copies of VitaraMaps inside the plugins directory.

4. **Copy the New Version**

* Copy the extracted VitaraMaps folder into the plugins directory of your MicroStrategy Web installation.\
  Example path: **\tomcat\webapps\MicroStrategy\plugins**

5. **Verify Folder Structure**

* Ensure that the folder structure appears correctly after installation.

![](<../.gitbook/assets/unknown (2) (1).png>)<br>

6. **Validate Version Folders**

* Confirm that only one version folder of VitaraMaps exists within both the style and source directories:\
  &#xNAN;**/Tomcat/webapps/MicroStrategy/plugins/VitaraMaps/style**

&#x20;     **/Tomcat/webapps/MicroStrategy/plugins/VitaraMaps/javascript/mojo/js/source**

* If multiple version folders are found, delete the entire VitaraMaps folder and redeploy the build.

7. **Apply License**

* Replace the license.txt file in the VitaraMaps folder with the license file provided to you.

8. **Restart the Web Server**

* Start IIS, Tomcat, or your equivalent web service.

9. **Clear Browser Cache**

* Clear browser caches and open dossiers/documents in a new incognito window to avoid issues from previously cached license files.

## Upgrading an Existing Installation

If you are upgrading an existing VitaraMaps installation, follow the steps below carefully.

### Step 1: Back Up Existing Customizations

Before upgrading, take a backup of all customization files from the existing installation.

VitaraMaps supports customization through the following files:

* **mappingLayers.txt** and its dependent files – Used to define and configure custom map layers.
* **global.txt** – Used to define color palettes, fonts, and other global configuration parameters.
* **customStyles.css** – Used to apply individual style customizations to the maps.

If you have created new custom maps that are not part of the default installation, make sure to back them up as well.

#### **File Locations:**

/webapps/MicroStrategy/plugins/VitaraMaps/custom/**global.txt**

/webapps/MicroStrategy/plugins/VitaraMaps/custom/**customStyles.css**

/webapps/MicroStrategy/plugins/VitaraMaps/custom/**mappingLayers.txt**

_**Note**: The plugins directory should contain only one folder named **VitaraMaps**. Do not keep backup copies of the VitaraMaps folder inside the plugins directory._

### Step 2: Install the New Version

1. **Download** the latest VitaraMaps web version from the provided link.
2. **Extract** the VitaraMaps folder from the ZIP file.
3. **Stop** the Web Server (IIS, Tomcat, or equivalent).
4. **Delete** the existing VitaraMaps folder under the plugins directory.
5. **Copy** the new VitaraMaps folder into the plugins directory of your MicroStrategy Web installation.
6. **Replace** the license.txt file in the new VitaraMaps folder with the license file provided to you.

**Restore** your backup files (**global.txt, customStyles.css, mappingLayers.txt**, and all its dependent files) to the following location:\
&#xNAN;**/webapps/MicroStrategy/plugins/VitaraMaps/custom/**

7. **Start** the Web Server.
8. **Clear** browser caches and access dossiers/documents from a new browser or incognito window to avoid issues related to previously cached license files.

## Important: Export Server Setup

If you are using the new Export Engine in MicroStrategy (available from version 2019 Update 2), you have the option of deploying VitaraMaps locally on the export server.The procedure is detailed here[ Export engine set up](https://community.microstrategy.com/s/article/New-Customization-Property-for-the-Export-Engine-Service?language=en_US)

* &#x20;Use the web version of VitaraMaps to copy files into the resources folder on the export server.
* Do not use the library or Workstation versions for export setup.

<br>
