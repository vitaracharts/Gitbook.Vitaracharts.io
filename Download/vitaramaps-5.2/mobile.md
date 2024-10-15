---
hidden: true
icon: mobile
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

# Mobile

## [Click Here](https://vitarachartsdownloads.azureedge.net/distributions/Maps/5.2.0.499/VitaraMapsMobile.zip) <a href="#download" id="download"></a>

### Download <a href="#download" id="download"></a>

* Download the **mobile version** of VitaraMaps.
* You can find the latest links for download from our download site at Main page

### Installation Steps <a href="#installation-steps" id="installation-steps"></a>

The downloaded file will be different from the web version and is called “_VitaraMapsMobile.zip_”

* Unzip the ‘_VitaraMapsMobile.zip_’file.
* This zip file will contain a folder named “_VitaraMapsMobile_”.
* Stop WebServer (IIS/Tomcat or equivalent)
* If you are an existing user of VitaraMaps, take backup of all the customization files (mappinglayer.txt, shape files, dictionary files, etc).
* Delete VitaraMapsMobile related folders under MicroStrategy mobile plugins directory (if any exist).
* **Please do not** keep any backup copies of VitaraMaps in the mobile plugins directory.
* Copy over the folder extracted from “_VitaraMapsMobile.zip_” file into the plugins folder of your MicroStrategy mobile installation. For instance if mobile server is installed under _c:\tomcat\webapps\MicroStrategyMobile_, you will place all folders under _c:\tomcat\webapps\MicroStrategyMobile_\*\*plugins\*\*
* Replace the folders/files you took backup (mappinglayer.txt, shape files, dictionary files, etc) into the appropriate location.
* Start WebServer.
* Connect your ipad to the mobile server

#### Configure Mobile Server Path <a href="#configure-mobile-server-path" id="configure-mobile-server-path"></a>

**Important** You need to update the config path and point to the web server using the steps below. After extracting the VitaraMapsMobile plugins into plugins folder of MicroStrategy Mobile server, navigate to the mobile configuration page:

**If MicroStrategy application is running on IIS/Windows**

```
https://<MicroStrategyMobileServer>/plugins/VitaraMapsMobile/config.aspx 
(ex: http://example.com/MicroStrategyMobile/plugins/VitaraMapsMobile/config.aspx)
```

**Setting Mobile Configuration URL to IIS server**

Setting mobile configuration url to Vitara Maps config helps to render Vitara Maps chart without internet access to the ipad/iphone.

On the page enter the path to the **MicroStrategy Web application** and click submit.

\


Below is the screenshot after configuring the mobile, and the web renders in this way.

\


* Clear cache in the app and Restart MicroStrategy iPad/iPhone app to see the changes.

**If MicroStrategy application is running on Tomcat/Linux**

```
https://<MicroStrategyMobileServer>/plugins/VitaraMapsMobile/config.jsp 
(ex: http://example.com/MicroStrategyMobile/plugins/VitaraMapsMobile/config.jsp)
```

**Setting Mobile Configuration URL to Tomcat/Linux Server**

Setting mobile configuration url to Vitara Maps config helps to render Vitara Maps chart without internet access to the ipad/iphone.

On the page enter the path to the **MicroStrategy Web application** and click submit.

\


Below is the screenshot after configuring the mobile, and the web renders in this way.

\


* Clear cache in the app and Restart MicroStrategy iPad/iPhone app to see the changes.
