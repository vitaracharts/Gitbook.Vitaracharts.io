---
description: Here's the list of all changes in each release (latest release first)
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Release Notes Maps

## 5.3.0

* BugFix: Threshold edit/creation doesn’t work with custom maps.
* BugFix: Incorrect 'Play by Attribute' Option Displayed in Map's Appearance Tab.
* BugFix: Missing 'Enable Layout Selector' Option in Map's Tab.
* BugFix: US Physical Map incorrectly display as "&\[Name]" instead of their actual names.
* BugFix: When we use a custom svg map which has background image and try to zoom it stays in same space.
* BugFix : Zoom Issue: Shapes Clipped, Background Unaffected.

## **5.1.1**

***

* Bugfix: Problem loading custom SVG maps on the workstation when the workstation is not connected to any environment.
* Bugfix: VitaraMaps Editor button is not enabled when using MSTR Workstation in connected mode.

## **5.1**

***

* Improvement: Feature to adjust transparency in the color picker.
* Bug fix: For percentage metrics threshold condition between is showing wrong values in the legend.

## **5.0**

***

* Enhancement: Default threshold in custom svg maps with background image will be transparent in new charts.
* Enhancement: Updated color picker to enable transparent color selection.
* Bug fix: Fixed missing dictionary file issue for African and European maps.
* Bug fix: Upgraded to use a newer version of a third party library (Apache commons) that fixes a potential security vulnerability.
* Bug fix: Default threshold color being changed when adding new threshold.
* Bug fix: Marker appear in the middle of the chart.
* Bug fix: Issues with dictionary files for Africa and Europe.

## **4.9.2**

***

* New Feature: Map layout tool export will also contain background image, can be integrated to maps via props.json file
* New Feature: Ability to include image from url via map layout tool.
* Bug fix: Fixed errors and added improvements while configuring using config.aspx and config.jsp
* Bug fix: Tooltip showing the text “false” on custom svg image maps.
* Bug fix: Layout tool copy id from another shape for images.

## **4.9.0**

***

* Enhancement: Revamped Vitara layout creation tool. Available at [Vitara Map Tool](https://cloud.vitaracharts.com/maptools/layoutCreator)
* Enhancement: Rotation Option for data labels.
* Enhancement: Improvements in Play axis UI configuration.
* Enhancement: Updated configuration files to warn and continue with the configuration in case of url is not reachable.
* Bug fix: Export Vitara charts to pdf is not working in MicroStrategy version 2021 5.1 (11.3.05).
* Bug fix: Fixed rendering issues in the edit mode of the web libarary in MicroStrategy2021 update-4.
* Bug fix: Error while doing ExportToPDF with MicroStrategy 2021 update 5.
* Bug fix: export not working with svg maps.
* Bug fix: Updated africa and europe tile maps to work with country codes.
* Bug fix: Edit button does not show up when 'can't find mapping layer' error occurs.
* Bug fix: Unable to click on tooltip links because the tooltip moves along with the mouse.
* Bug fix: Tooltip editor for VitaraMap does not have the option to format.

## **4.6.0**

***

* New Feature: Thresholds can be set using attributes.
* Bug Fix: File and folder permissions fix included for linux systems.
* Bug Fix: Resizable property editor changes.
* Bug Fix: Export issues with library and using resource directory deployment.
* Bug Fix: Dual rendering issues in IE.
* Bug Fix: Exported PDF shows black background.
* Bug Fix: Tiles map is not rendering in the web Library and showing a runtime error.
* Bug Fix: Mobile and library configuration for aspx server not working.
* Bug Fix: The legend does not show metric format (condensed). Instead it is incorrectly showing non-condensed format, and also adding B.
* Bug Fix: Maps in web documents are not loading in Android, JavaScript errors occur.

## **4.1.2**

***

* Bug Fix: svg map type failing to render due to uncaught error.
* Bug Fix: Tile map is failing to render due to uncaught error.
* Bug Fix: Error "getBackwardCompatibleFiveScaleThresholds is not a function".
* Bug Fix: Tile Map not working in combination with Vitara Charts.

## **4.1.1**

***

* Bug Fix: Cross site scripting security vulnerability via import data for metric data.
* Bug Fix: invalid data like non number characters within metric columns are nullified and the specific columns meta info is updated.

## **4.1.0**

***

* New Feature: Implemented Tile Map Support.
* New Feature: Implemented attribute based Map Support.
* New Feature: Implemented Iphone Support for VitaraMaps.
* New Feature: Implemented Support for Android Map Mobile and Ipad Map Mobile (Library and Regular Mobile App).
* Bug Fix: All Vitara charts: Threshold editor is giving error message if we have a map chart in dossier.
* Bug Fix: Map chart in mobile: If we resize the map chart on the mobile, it is showing an error.

## **Note:**

Add shape file extension as .json instead of “.geo.json” for attribute-based maps.\
To configure Mobile and Library, go to config.jsp and fill the URL of web Microstrategy as below: [http://139.59.83.206:8080/MicroStrategy](http://139.59.83.206:8080/MicroStrategy)\
For custom map file to be loaded in mobile you should have “dictionary” key corresponding to each layer in mappingLayers.txt.

* Bug Fix: Export to pdf is not working from Library.
* Bug Fix: Map Chart: Exported PDF file is not showing pallet colors.
* Bug Fix: Map chart: Edit property window is going behind other panels and unable to move.

## **4.0.1**

***

* Bug Fix: On adding vitaramaps with vitaraChart, legend in VitaraCharts are getting bold.
* Bug Fix: Map chart in combination with vitara charts showing encoded text in the color selection box.
* Bug Fix: Legend colors of other vitara charts in the dashboard get changed when any vitara chart is converted to map chart
* Bug Fix: Included Firefox issues.

### **4.0.**

***

* Bug Fix: If Vitara Charts used first and maps later then map works without license validation.
* Bug Fix: Map Chart not rendering properly for documents (Metrics with space as first character were missing from plot).
* Bug Fix: Fixed: Default thresholds backwards compatibility.
* Bug Fix: Fixes related to compatibility issues with VitaraCharts.
