---
hidden: true
icon: artstation
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

# Workstation

## [Click Here](https://vitarachartsdownloads.azureedge.net/distributions/Maps/5.2.0.499/VitaraMaps.zip) <a href="#download" id="download"></a>

### Download <a href="#download" id="download"></a>

* Download the **desktop version** of VitaraMaps.
* You can find the latest links for download from our download site at Main page

### License <a href="#license" id="license"></a>

On MicroStrategy Desktop and Workstation we no longer enforce license validation. So use of VitaraMaps is freely permitted on these applications.

### Deployment Steps <a href="#deployment-steps" id="deployment-steps"></a>

**1. Offline Mode:**

* Open an existing MicroStrategy dossier or choose to create a new dossier.
* You will see a “​+”​ sign to add visualizations
* Now point to the VitaraMaps.zip that you downloaded in your local machine .
* Once the vitara visualization imported successfully, you will see a message stating all the custom visualizations imported successfully.

**2. Connected to MicrostrategyLibrary Server:**

* In order to use the workstation in “connected to environment” mode, you must install the ViaraMaps plugin on the MicroStrategyLibrary server to which workstation is connected. Please follow the MicroStrategyLibrary installation steps here: https://docs.vitaracharts.com/installationMaps/mapsLibraryInstallationSteps.html
* When upgrading an existing installation, make a backup of any alterations made to the existing VitaraMaps installation, such as changes made to the mapping layer, dictionaries, and so on.
* In addition, you must install the VitaraMaps plugin locally on your PC. Navigate to your local machine’s MicroStrategy Workstation installation folder. Unzip the downloaded VitaraMaps.zip file in the \Code\plugins\ folder. For example, on a Windows PC, the path to the VitaraMaps plugin deployment folder is shown below. C:\Program Files\MicroStrategy\Workstation\Code\plugins\*
* Configure MobileLibrary Server Path: In any web browser navigate to the library configuration page. Below is the example URL to open the configuration web page.

```
https://<MicroStrategyLibraryServer>/plugins/VitaraMaps/config.jsp 
(Example: ​http://example.com/MicroStrategyLibrary/plugins/VitaraMaps/config.jsp)
```

Below is a screenshot of the library configuration page. On this page, enter the path to the MicroStrategy Web application (not the library) and click submit.
