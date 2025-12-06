# Installing VitaraMaps on MicroStrategy desktop/Workstation

### Download

* For both desktop and workstation applications, download the desktop version of VitaraMaps.
* You can find the latest links for download from our download site at[ Main page](https://www.vitaracharts.com/ms-product-downloads)

![](<../.gitbook/assets/unknown (3) (1).png>)

### License

On MicroStrategy Desktop and Workstation we no longer enforce license validation. So use of VitaraMaps is freely permitted on these applications.

“Ensure there are no existing or old build files in your local machine’s Workstation folder. Delete any such files completely before deploying a new build in Workstation.”

**"C:\Program Files\MicroStrategy\Workstation\Code\plugins”**

(**Note**: The path may vary depending on the operating system or version.)

## Deployment Steps

There are two ways to deploy in Offline Mode:

### 1.UI Installation- Deployment from adding directly plugin to the ‘+’sign:

* Ensure you have downloaded the desktop version (Vitara Maps.zip) specifically built for[ Workstation](https://www.vitaracharts.com/product-downloads).
* Open an existing MicroStrategy dossier or create a new one.
* You will see a ​+​ sign to add visualizations.

![](<../.gitbook/assets/unknown (1).jpeg>)

* Click on the ‘+’ sign, and a small import visualization window will open. Select the downloaded zip file.

![](<../.gitbook/assets/unknown (5) (1).png>)

* Once the Vitara visualization is successfully imported, you will see a message stating that all custom visualizations have been imported successfully.

![](<../.gitbook/assets/unknown (2).jpeg>)

### 2.Manual Installation- Deployment by Extracting and Pasting the Folder:

* Download the desktop version zip file from[ here](https://www.vitaracharts.com/product-downloads).
* Once the file is downloaded, extract the zip file to your specified location. You will find that under the Vitara Maps folder, there is another Vitara Maps folder containing several subfolders. Move the inner folder that contains the files.
* ![](<../.gitbook/assets/unknown (8) (1).png>)

<br>

* Paste the extracted folder into the **\Microstrategy\Workstation\Code\plugins** path on your local machine.

![](<../.gitbook/assets/unknown (9) (1).png>)

* Open Workstation and create a new dossier. You should see the **Vitara Maps** in the custom option.

### Connected to MicroStrategyLibrary Server

When using MicroStrategy Workstation in Connected to Environment mode, the VitaraMaps plugin must be installed both on the MicroStrategy Library Server and on your local Workstation.

#### 1. Deploy VitaraMaps on the MicroStrategy Library Server

To use VitaraMaps with MicroStrategy Workstation, ensure that the VitaraMaps plugin is deployed on the MicroStrategy Library Server that your Workstation connects to.

Follow the installation steps provided in the official documentation:\
[https://docs.vitaramaps.com/installation/libraryInstallSteps.html](https://docs.vitaramaps.com/installation/libraryInstallSteps.html)

#### 2.  VitaraMaps Locally on Workstation

In addition to the server installation, the VitaraMaps plugin must also be deployed locally on your machine.

* Go to the MicroStrategy Workstation installation folder on your local system.
* Navigate to the following path:

"**C:\Program Files\MicroStrategy\Workstation\Code\plugins”**&#x20;

* Unzip the downloaded VitaraMaps.zip file into this folder.

#### Configure MobileLibrary Server Path:

&#x20;1\. Open a web browser and navigate to the Library configuration page using the URL format below:

&#x20;**https://www.example.com/MicroStrategyLibrary/plugins/VitaraMapsLibrary/config.jsp**

(Replace “example.com” with the actual path of your **Library** server.)

2. On the configuration page, enter the path to your **MicroStrategy Web** application (not the Library) and click Submit.\
   Example: **https://\[your-web-server-path]/MicroStrategy**

(Replace this with the actual path of your **Web** server.)

3. Once configured successfully, the page will confirm the configuration status as shown in the screenshot.

![](<../.gitbook/assets/unknown (10) (1).png>)

<br>
