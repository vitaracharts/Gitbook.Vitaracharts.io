# Installing on MicroStrategy Desktop/Workstation

## Download <a href="#download" id="download"></a>

* For both desktop and workstation applications, download the **desktop version** of VitaraCharts.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Click on the ‘+’ sign, and a small import visualization window will open. Select the downloaded zip file.

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Once the Vitara visualization is successfully imported, you will see a message stating that all custom visualizations have been imported successfully.

<figure><img src="../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

## **2.Manual Installation- Deployment by Extracting and Pasting the Folder:**

* Download the desktop version zip file from [here](https://www.vitaracharts.com/product-downloads).
* Once the file is downloaded, extract the zip file to your specified location. You will find that under the Vitara Charts folder, there is another Vitara Charts folder containing several subfolders. Move the inner folder that contains the files.&#x20;

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

* Paste the extracted folder into the _**\Microstrategy\Workstation\Code\plugins**_ path on your local machine.&#x20;

<figure><img src="../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

* Open Workstation and create a new dossier. You should see the Vitara charts in the custom option.

### Connected to MicroStrategyLibrary Server

When using MicroStrategy Workstation in Connected to Environment mode, the VitaraCharts plugin must be installed both on the MicroStrategy Library Server and on your local Workstation.

**1. Deploy VitaraCharts on the MicroStrategy Library Server**

To use VitaraCharts with MicroStrategy Workstation, ensure that the VitaraCharts plugin is deployed on the MicroStrategy Library Server that your Workstation connects to.

Follow the installation steps provided in the documentation:

[https://docs.vitaracharts.com/install-docs/installing-on-microstrategy-library](https://docs.vitaracharts.com/install-docs/installing-on-microstrategy-library)&#x20;

**2.  VitaraCharts Locally on Workstation**

In addition to the server installation, the VitaraCharts plugin must also be deployed locally on your machine.

* Go to the MicroStrategy Workstation installation folder on your local system.
* Navigate to the following path:

**"C:\Program Files\MicroStrategy\Workstation\Code\plugins”**

* Unzip the downloaded VitaraCharts.zip file into this folder.

### **Configure MobileLibrary Server Path:**

1\. Open a web browser and navigate to the Library configuration page using the URL format below:

**https://www.example.com/MicroStrategyLibrary/plugins/VitaraCharts/config.jsp**

(Replace “**example.com**” with the actual path of your **Library** server.)

2\. On the configuration page, enter the path to your MicroStrategy Web application (not the Library) and click Submit.

* Example: **https://\[your-web-server-path]/MicroStrategy**

(Replace this with the actual path of your **Web** server.)

* Once configured successfully, the page will confirm the configuration status as shown in the screenshot.

![](<../.gitbook/assets/unknown (17).png>)&#x20;
