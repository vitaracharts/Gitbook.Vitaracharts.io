---
hidden: true
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

# Error while trying to export charts to PDF

**We are seeing errors while trying to export to PDF**

Please note MicroStrategy only supports export to PDF of custom visuals from dossiers. When you export report services documents to PDF, custom visuals will be shown as a grid.

**For MicroStrategy server versions 2019 Update 2 or newer**

Please note that starting with MicroStrategy version 2019 Update 2, MicroStrategy has made changes to how the pdf export works and how it should be set up for custom visuals. You need to set up the visualization files locally on the export server.

[Instructions on how to set up local resource folder](https://www2.microstrategy.com/producthelp/Current/InstallConfig/en-us/Content/export\_engine\_local\_resource\_loading.htm)

**IMPORTANT** : Please use the web version of the VitaraCharts to set up the local resource folder on the export server

There are further troubleshooting steps made available by MicroStrategy. You can find them here

[Troubleshooting the new export engine](https://community.microstrategy.com/s/article/Troubleshooting-the-New-Export-Engine-in-2019-Update-2?language=en\_US)

**For older MicroStrategy Servers (prior to MicroStrategy 2019 update 2)**

With dossiers, you may also see error messages when the export happens. For instance, the message could be something like **Failed to display visualization: HCStackedBarChart because failed to get pluginsVisList from** **Failed due to NetworkError: Failed to execute ‘send’ on ‘XMLHttpRequest’: Failed to load**

This is typically because of network configuration/permissions. You can also confirm this by trying to export a dossier with some other custom visual (like the D3WordCloud provided by MicroStrategy in the first row of the custom visuals). You will see the export fail with the same reason.

The access issues may arise from the type of user and authentication used on both machines. Here are couple of relevant links from MicroStrategy that describe this problem and also suggest some workarounds.

[MicroStrategy Community - Export error](https://community.microstrategy.com/s/question/0D544000077J4yxCAC/error-when-exporting-to-pdf-a-dossier-with-geospatial-visualization?language=en\_US)

[MicroStrategy Community - Windows Authentication export issue](https://community.microstrategy.com/s/article/KB442054-Unable-to-Render-ESRI-Map-when-Exporting-Dashboard-Dossier-as-PDFs-while-Windows-Authentication-Mode-Configured?language=undefined)

Please review and let us know if these apply to your case. In this scenario it is best to contact MicroStrategy to make sure best practices are being followed for setting up the network for export.

If the export is failing because of a different symptom then please contact Vitara support.
