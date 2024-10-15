---
hidden: true
icon: globe-wifi
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Web Install

## [Click Here](https://vitarachartsdownloads.azureedge.net/distributions/Maps/5.2.0.499/VitaraMaps.zip) <a href="#download" id="download"></a>

## Download <a href="#download" id="download"></a>

* Download the **web version** of VitaraMaps.
* You can find the latest links for download from our download site at Main page

### Installation Steps <a href="#installation-steps" id="installation-steps"></a>

* Download the web version from the link above.
* Stop WebServer (IIS/Tomcat or equivalent).
* If you are an existing user of VitaraMaps chart, take backup of the “license.txt” file and “custom” folder (available inside the VitaraMaps folder). The “custom” folder will contain mapping layer.txt file, shape files, dictionary files and other customization files you are using currently in the VitaraMap visualization.
* Delete the VitaraMaps folder under plugins directory if one exists.
* Copy the new version of the VitaraMaps build (zip file) into the plugins folder. Extract the VitaraMaps folder from the zip file.
* After extracting delete the zip file.
* **Please do not**​ keep any backup copies of VitaraMaps in the plugins directory.
* Copy over the new version of the VitaraMaps folder into the plugins folder of your MicroStrategy web installation. For instance if Web is installed under ​_c:\tomcat\webapps\MicroStrategy_, you will place VitaraMaps under ​_c:\tomcat\webapps\MicroStrategy​\​plugins_
* REPLACE the license.txt file in the VitaraMaps folder with the license file provided to you.
* If you are a existing user of VitaraMaps, replace all the files which you took backup into the appropriate location.
* Start WebServer.
* Flush any browser caches and access the dossier/documents from a new browser window (to avoid any issues with a previously used license file).

**Important** **For IIS users** : If you plan to also deploy the mobile app, in order for the mobile app to load the maps definition files the client will need to be able to access VitaraMaps folder. If you have windows authentication turned on, then the client access will be restricted. In order to overcome this problem, you will have to turn on ‘Anonymous Authentication’ for just the VitaraMaps and subfolder under plugins. You can do this in the IIS manager.

**Important : Set up info for the MicroStrategy export server**

If you are using the new export engine on MicroStrategy (available starting 2019 update 2) you have the option of deploying VitaraMaps locally on the export server. The procedure is detailed here [Export engine set up](https://community.microstrategy.com/s/article/New-Customization-Property-for-the-Export-Engine-Service?language=en\_US)

Use this web version of VitaraMaps to copy them to the resources folder on the export server. Please do not use the library or mobile version.
