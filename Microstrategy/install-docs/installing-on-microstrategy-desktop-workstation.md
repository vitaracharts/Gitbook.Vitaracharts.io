---
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

# Installing on MicroStrategy Desktop/Workstation

## Download <a href="#download" id="download"></a>

* For both desktop and workstation applications, download the **desktop version** of VitaraCharts.
* You can find the latest links for download from our download site at [Main page](https://www.vitaracharts.com/ms-product-downloads)

## License <a href="#license" id="license"></a>

<mark style="color:blue;">On MicroStrategy Desktop and Workstation we no longer enforce license validation. So use of VitaraCharts is freely permitted on these applications.</mark>

**Ensure there are no existing or old build files in your local machine’s Workstation folder. Delete any such files completely before deploying a new build in Workstation.**

**\*\Microstartegy\Workstation\Code\plugins\***

## Deployment Steps <a href="#deployment-steps" id="deployment-steps"></a>

There are two ways to deploy in Offline Mode:

## **1.UI Installation- Deployment from adding directly plugin to the ‘+’sign:**

* Ensure you have downloaded the desktop version (Vitara Charts.zip) specifically built for [Workstation](https://www.vitaracharts.com/product-downloads).
* Open an existing MicroStrategy dossier or create a new one.
* You will see a ​+​ sign to add visualizations.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

* Click on the ‘+’ sign, and a small import visualization window will open. Select the downloaded zip file.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

* Once the Vitara visualization is successfully imported, you will see a message stating that all custom visualizations have been imported successfully.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

## **2.Manual Installation- Deployment by Extracting and Pasting the Folder:**

* Download the desktop version zip file from [here](https://www.vitaracharts.com/product-downloads).
* Once the file is downloaded, extract the zip file to your specified location. You will find that under the Vitara Charts folder, there is another Vitara Charts folder containing several subfolders. Move the inner folder that contains the files.&#x20;

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

* Paste the extracted folder into the _**\Microstrategy\Workstation\Code\plugins**_ path on your local machine.&#x20;

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

* Open Workstation and create a new dossier. You should see the Vitara charts in the custom option.

## Connected to MicroStrategyLibrary Server <a href="#connected-to-microstrategylibrary-server" id="connected-to-microstrategylibrary-server"></a>

* In order to use the workstation in “connected to environment” mode, you must install the ViaraCharts plugin on the MicroStrategyLibrary server to which workstation is connected. Please follow the MicroStrategyLibrary installation steps here https://docs.vitaracharts.com/installation/libraryInstallSteps.html
* In addition to this, you have to deploy the VitaraCharts plugin locally on your machine. Go to the MicroStrategy Workstation installation folder in your local machine. Navigate to _**\Code\plugins**_\ folder and unzip downloaded VitaraCharts.zip file here.\
  For example, in the windows machine below is the path of the folder where you have to deploy the VitaraCharts plugin.\
  _C:\Program Files\MicroStrategy\Workstation\Code\plugins\*_
*   **Configure MobileLibrary Server Path:** In any web browser navigate to the library configuration page. Below is the example URL to open the configuration web page.\


    ```
    https://<MicroStrategyLibraryServer>/plugins/VitaraCharts/config.jsp 
    (Example: ​http://example.com/MicroStrategyLibrary/plugins/VitaraCharts/config.jsp)
    ```

    Below is a screenshot of the library configuration page. On this page, enter the path to the MicroStrategy Web application (not the library) and click submit.

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
