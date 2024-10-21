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

# Workstation

### Known Issues in Workstation <a href="#known-issues-in-workstation" id="known-issues-in-workstation"></a>

#### Issues fixed in 5.1.4.047 <a href="#issues-fixed-in-514047" id="issues-fixed-in-514047"></a>

**1. Edit button:** When we connect the workstation to the environment, Vitarcharts don’t show the edit button.\
**2. Changes to external files:** Changes to external file (global.txt, IBCSGlobal.txt, custom data markers) are not loaded when using MSTR Workstation in connected mode.\
The list of all changes in 5.1.4 can be found here\
https://docs.vitaracharts.com/changeLog/revisionHistory.html

#### Known issues in the 5.1.4.047 version: <a href="#known-issues-in-the-514047-version" id="known-issues-in-the-514047-version"></a>

1. When we connect the workstation to the environment, and try to create a new VitaraChart, the chart will show an error message - _“Warning: Javascript class not found.”_ To overcome this issue please deploy the build locally in your machine.\
   For deployment of VitaraCharts into the MicroStrategy Workstation, please refer to the Workstation [installation guide](../support/install-docs/).
2. VitaraCharts icons are not working in the connected mode.
