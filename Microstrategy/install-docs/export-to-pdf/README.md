# Export to PDF

#### Set up and installtion: <a href="#set-up-and-installtion" id="set-up-and-installtion"></a>

With **MicroStrategy 2019 update 2**, modifications have been made to the way that custom plugins are configured for PDF export. Details are available at the following link.

[Export engine local resource set up](https://www2.microstrategy.com/producthelp/Current/InstallConfig/en-us/Content/export_engine_local_resource_loading.htm)

[Troubleshooting PDF export issues](https://community.microstrategy.com/s/article/Troubleshooting-the-New-Export-Engine-in-2019-Update-2?language=en_US)

Please use the **web version of Vitara Charts** to deploy to the local resource folder (as specified in the above link’s setup). Please use Vitara Charts version 4.4.4 (or newer) to ensure full support for the use of the local resource folder.

## Other FAQs related to export to PDF: <a href="#other-faqs-related-to-export-to-pdf" id="other-faqs-related-to-export-to-pdf"></a>

### **We are getting the following error when we export vitara charts to PDF,&#x20;**_**Failed due to NetworkError: Failed to execute ‘send’ on ‘XMLHttpRequest’: Failed to load**_**. How do you resolve this?**

This has happened in a few other customer environments, and it is a network/configuration issue. You can quickly verify this by exporting any other chart from the gallery (not just VitaraChart). They will fail in the same manner. To export, the pdf engine must be able to connect to the Web server and have access to all plugin files. Connecting from the system where the pdf server is installed may cause access concerns. The type of user and authentication used on both devices may cause access concerns. Here are a couple of important MicroStrategy links that outline the issue and provide potential remedies.\
[Error while exporting](https://community.microstrategy.com/s/question/0D544000077J4yxCAC/error-when-exporting-to-pdf-a-dossier-with-geospatial-visualization?language=en_US)

[Window Auth error while exporting](https://community.microstrategy.com/s/article/KB442054-Unable-to-Render-ESRI-Map-when-Exporting-Dashboard-Dossier-as-PDFs-while-Windows-Authentication-Mode-Configured?language=undefined)

The configuration issue is best dealt with from the MicroStrategy side (i.e opening a case with MicroStrategy) because they can provide the best way to set up the network.

**We are getting an Error with&#x20;**_**“Http Status Code: 0”**_**&#x20;in the exported PDF of vitara charts. How to solve this problem?**

The error appears to indicate a configuration problem. To enable the export, the PDF engine must be able to connect to the Web server and access all plugin files. Connecting from the system where the pdf server is installed may cause access concerns. The type of user and authentication used on both devices may cause access concerns. If the VitaraCharts folder on the web server has been configured with different access privileges than the rest of the MicroStrategy Web installation. If that’s the case, you might try changing their access rights to match the rest of the folders.

**We are getting an error with&#x20;**_**“Http Status Code 401”**_**&#x20;in the exported pdf file.**

The error (401) indicates that there is a problem with accessing the web server. In order to create the PDF document, the PDF export server must communicate with the web server. So the first step would be to ensure that the PDF export engine (which should be on the same computer as the intelligence server) can reach the web server (through the network). When the configuration is not done correctly, not only VitaraCharts but also any of the custom chart plugins will not function properly. If the connectivity troubles persist, it may be preferable to contact MicroStrategy for network configuration assistance.

**When I export to pdf, the Vitara Charts get cut off after one page. Doing the export with a regular MSTR Grid works fine and splits the grid over more pages. How to split vitara charts into multiple pages?**

Unfortunately, MicroStrategy does not support exporting several pages of customised visuals. Essentially, exporting custom visuals is similar to taking a screenshot; whatever is displayed within the context of the website will be exported. Of course, you can adjust the page parameters during export (as you have already attempted) to ensure that your page is as large as feasible. We’ve also requested that MicroStrategy improve their API to support several pages of bespoke visual export. The case number is 358341.

**How can we generate the export engine logs?**

Please check the following link for info on export engine logs\
[Troubleshooting the export engine](https://community.microstrategy.com/s/article/KB442425-Troubleshooting-the-MicroStrategy-2019-Export-Engine?language=en_US)

**Exports come with a&#x20;**_**black background**_**&#x20;and nothing else is displayed.**

The issue is caused by network setup (or possibly by web server configuration). Could you please try to access vitaraGlobal.css from the server where the export engine is running? A sample URL for doing so is shown below: https://xyz.com/MicroStrategy/plugins/VitaraCharts/style/vitaraGlobal.css Simply copy and paste the URL into your browser (this must be done on the export engine machine). If that returns a proper answer (i.e. displays the CSS file in the browser window or prompts you to download the file), the setting is correct and we must hunt elsewhere for the problem. If it fails to load, this must be addressed first (by your web/network administrator). If this access issue is resolved, the black background issue should be resolved.\
You can also check MicroStrategy’s troubleshooting tech note for export:\
[Troubleshooting the new export engine](https://community.microstrategy.com/s/article/Troubleshooting-the-New-Export-Engine-in-2019-Update-2?language=en_US)\
This talks about the ‘Request Failed’ errors and wants the user to check ‘to Make sure the account used to start the export engine has read-access to the file’.

**When we exporting Vitara Chart in the result from Dossier to PDF we noticed the below issues:**

```
     1.Some Metric Value Data labels are missing.
     2.Y-Axis values also change. The size of the page used in the pdf layout will be different from what is seen on the screen. With export, the summary view of the dossier is generated on one page and then a separate page is created for each chart on the same chapter/sheet. The separate page size (aspect ratio) will not exactly match the aspect ratio of the visual as seen in the dossier. For this reason sometimes vitara charts may include some extra data labels or disappear existing data labels in the PDF. Sometimes in the original view some rows are partially cut-off while they are seen in the pdf export.
```

**What are the MicroStrategy compatible environments for export to PDF to work in Vitara charts?**

Only with version 10.6 has MicroStrategy supported the export of custom visuals. Previously, simply a grid would be exported. Export to PDF from online dossiers, web library, and workstation is supported in vitara charts.

Custom graphics from Documents cannot be exported by MicroStrategy. This is a shortcoming in MicroStrategy for which we have repeatedly requested a fix.

**What is the workflow of VitaraCharts export to PDF?**

It’s a straightforward one-way trade. VitaraCharts’ scope is entirely contained to the web-server and makes no requests to the i-server or any other service. When you export a dashboard/dossier to PDF, the intelligence server’s PDF service runs the dashboard and takes a screenshot of the output to include in the PDF.

**What are the basic troubleshooting steps I can perform if I have problems with export to PDF?**

i) Only with version 10.6 has MicroStrategy supported the export of custom visuals. Check the version of MicroStrategy you’re using.

ii) Export to PDF in any custom visualisations will only function with dossiers. When you try to export data from Web documents to PDF, you will obtain data in a grid format.

iii) You can export any other custom visual from the gallery (that Vitara does not provide) from a dossier.This helps determine whether the problem is with exporting any custom visuals (suggesting a configuration issue) or a VitaraCharts-specific issue.

**In Dossiers/documents does VitaraCharts support export to Excel?**

No, Exporting to excel is not supported.
