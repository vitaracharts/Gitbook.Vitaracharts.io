# Installing VitaraCharts on MicroStrategy Library

**Download**

* Download the library version of VitaraCharts from the official download page.
* You can find the latest version links on the VitaraCharts[ Main Page.](https://www.vitaracharts.com/ms-product-downloads)

![](<../.gitbook/assets/unknown (18).png>)

### 2. Installation Steps

Follow the steps below to install VitaraCharts for MicroStrategy Library.

#### &#x20;**Steps**

1. **Download** the **VitaraChartsLibrary.zip** file.\
   This ZIP contains:

* A main folder named **VitaraCharts**
* Separate folders for each Vitara visualization (around **30+ folders** total)

2. **Unzip** the contents of the **VitaraChartsLibrary.zip** file.\
   You will see multiple folders (one for each chart type).
3. **Stop** the Web Server (IIS, Tomcat, or equivalent).
4. **Delete** any existing **VitaraCharts**-related folders under the **MicroStrategy Library plugins** directory.\
   ⚠️ **Important**: Do not keep backup copies of VitaraCharts within the plugins directory.
5. **Copy** all the folders extracted from the **VitaraChartsLibrary.zip** file into the plugins folder of your MicroStrategy Library installation.\
   \
   **Path**:  C:\tomcat\webapps\MicroStrategyLibrary\plugins\\
6. After deployment, your plugins directory should contain multiple VitaraCharts folders (one per visualization).

![library install directory](https://vitaracharts.github.io/assets/img/libraryInstallDirectory.png)

* **MicroStrategy 2021 Update 4 and newer versions**\
  From MicroStartegy 2021 update 4 version we can edit dossiers in the web library. So you have to provide license file in the library deployment also.
* &#x20;**REPLACE** the **license.txt** file in the _**webapps/MicroStrategyLibrary/plugins/VitaraCharts/**_ folder with the license file provided to you.
* **Start​** the WebServer.
* **Clear any browser caches** and access the dossier/documents from a new browser window (to avoid any issues with a previously used license file)

## Configure Mobile Library Server Path <a href="#configure-mobile-library-server-path" id="configure-mobile-library-server-path"></a>

Starting with version **4.7** the following steps are **always** required.

After extracting the **VitaraChartsLibrary** plugins into plugins folder of MicroStrategy Library server, navigate to the library configuration page. Below are are the example URLs to open the configuration web page.

## **MicroStrategy Installation on IIS/Windows versions**

```
https://<MicroStrategyLibraryServer>/plugins/VitaraCharts/config.aspx 
(Example: ​http://example.com/MicroStrategyLibrary/plugins/VitaraCharts/config.aspx)
```

## **MicroStrategy Installation on Tomcat/Linux versions**

```
https://<MicroStrategyLibraryServer>/plugins/VitaraCharts/config.jsp 
(Example: ​http://example.com/MicroStrategyLibrary/plugins/VitaraCharts/config.jsp)
```

1. On the configuration page, enter the path to your MicroStrategy Web application (not the Library) and click Submit.
2. Once successfully configured, the page will confirm the setup with a success message. ![](https://docs.vitaracharts.com/~gitbook/image?url=https%3A%2F%2F230207405-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FOuiTPVEbVQnzR38vviPf%252Fuploads%252F8QcQ1SbHigXqdWbWe9Wd%252Funknown.png%3Falt%3Dmedia%26token%3De91584c3-4a4f-4015-8772-69592df9af78\&width=300\&dpr=4\&quality=100\&sign=f920b8b1\&sv=2)

**Notes:**

* Setting the Web configuration URL enables **VitaraCharts** to render without internet access on iPad/iPhone.
* **Clear the cache** and restart the MicroStrategy Library Mobile App on your device to apply changes.
* For detailed instructions on clearing cache [Click here](https://docs.vitaracharts.com/faq/how-to-fix-mobile-rendering-issues#id-2.-clear-mobile-library-application-cache)

#### **Note:** Starting with version 5.3.6, a new utility named Health Tool has been introduced.

This tool provides a centralized interface to verify the correct deployment of the Vitara Charts plugin and helps identify potential configuration or compatibility issues.

👉[ Click here ](health-tool.md)to access the **Health Tool**.

