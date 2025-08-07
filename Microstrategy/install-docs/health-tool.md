# Health Tool

## Health Tool (Introduced in Version 5.3.6)

Starting with version 5.3.6, a new utility named Health has been introduced. This tool provides a centralized interface to verify the correct deployment of the VitaraCharts plugin and helps identify potential configuration or compatibility issues.

It simplifies the troubleshooting process by giving a comprehensive overview of the plugin’s deployment status and environment integrity.

### &#x20;Key Areas Covered

**1. Version Compatibility**

Validates whether the installed VitaraCharts version is compatible with the current MicroStrategy Web or Library version.

* Checks compatibility with MicroStrategy Web and Library
* Ensures proper support for Maps integration
* Verifies overall version alignment

**2. Deployment or Build Structure**

Ensures all required files and folders are correctly deployed under the plugin directory.

* Validates build type and platform
* Checks plugin folder structure
* Confirms correct folder version
* Identifies any duplicate or misplaced folders

**3. File Integrity Check**

Confirms that all plugin files are intact and not corrupted.

* Verifies file existence
* Detects file corruption or missing files

**4. Custom File Validation**

Ensures custom configuration files are present and correctly structured.

* Verifies presence of files like CustomStyles.css and global.txt
* Confirms customization rules are followed
* Checks font links and other references in custom files

**5. License Verification**

Validates the presence and status of the license file.

* Confirms the license file exists
* Flags if the license is missing or invalid

**6. Mobile Configuration**

&#x20;Confirms if the required configurations are set for mobile compatibility and integration with MicroStrategy mobile apps.

* Validates mobile and Library configuration
* Confirms required custom folders and mobile-specific settings are properly set

#### File Access Paths

* **Web:**\
  /MicroStrategy/plugins/VitaraCharts/utils/health.html
* **Web Library:**\
  /MicroStrategyLibrary/plugins/VitaraCharts/utils/health.html
* **Mobile:**\
  /MicroStrategyMobile/plugins/VitaraCharts/utils/health.html

#### Example Scenario: Custom Files Validation Messages

In the screenshot below, a warning message is displayed under the Custom Files Validation section of the **Health** Utility.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdAzozbJvkDRV54-TOYn5p4nOtyUGEtrrW76qUggn9hC1h0_baHzhMiCVwiEY-4nYbk_Qt3tMde423SI5goEEoyCxxIBUiOQzmFH05_er519QTbgX-h-y5wgbY6sn2FPRjx-MTw?key=x_xCMrMz4CVyQ8avpvVkfA" alt=""><figcaption></figcaption></figure>

\
The Health Utility provides visual indicators to help users quickly identify and troubleshoot issues:

* <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc0yXbA2iqT-mlByWyti52YCsdSAcKh0g-fUGwsAkkr3BMghXf6Tg35KAR_zmuqKKOIW_AO-vYtOWYzZkpa5Wq0zdhY5kLd9IN7lBumFCw_x3_4KlDsSxSQLLWCcN5G48YUrJXq?key=x_xCMrMz4CVyQ8avpvVkfA" alt="" data-size="line"> Errors are shown with a red circular icon.
* ⚠️ Warnings are marked with a triangle warning icon.
* 💡 A bulb icon appears next to each issue, offering suggested solutions.

By reviewing these messages and icons, users can take the necessary actions to resolve configuration problems and ensure the plugin is functioning correctly.

If the issue persists, users can click the **Copy to Clipboard** option to copy the error details and share them with the **Vitara Support Team** for further assistance.
