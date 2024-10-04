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

# Text Node

### Vitara Text Node <a href="#vitara-text-node" id="vitara-text-node"></a>

Vitara’s text node chart can be used to provide space between visualisations, show tittles, display images, or present IBCS chart specific features.

#### Inputs <a href="#inputs" id="inputs"></a>

Attributes - At Least one attribute needs to be provided for the visualization.\
Metrics - No metrics needed.\
Use as Filter Option - Not Available

#### 1. Space Between Visualizations <a href="#id-1-space-between-visualizations" id="id-1-space-between-visualizations"></a>

To acquire the desired appearance and feel for the VI dashboard, add to dossier to make space between visualisations and adjust for size.The dashboard example below features a spacer between each visualisation and at the title area.

#### 2. Show Filter Selection Elements <a href="#id-2-show-filter-selection-elements" id="id-2-show-filter-selection-elements"></a>

Vitara text node chart can be used to display the filter selection when we utilize the filter panel to filter the data in the dossier. Drag and drag the identical property that you used in the filter panel into the Vitara text node chart’s “Editor” panel. When you move the cursor over the chart, a “Edit” button will appear. When you click the “Edit” button, a pop-up window appears. In the macro editor window, enter “&” in the “Text Properties” menu. All potential macros, or the properties applied to the text node, will be displayed in the popup window.

\


In the below screenshot vitara text node chart is showing the filter selction used in the dossier.\


#### 3. Tittles and Background Images <a href="#id-3-tittles-and-background-images" id="id-3-tittles-and-background-images"></a>

Text node chart can be used to show an image in the dossier. The steps to set a background image for all Vitara charts are explained in the following document backgroundImage.

To display the title of the dossier or document, we can utilize the Vitara text node chart as a text container. Using the Vitara text node chart, we can add a stunning title to our dossier or paper in addition to the background image feature.

#### 4. IBCS Specific Usage <a href="#id-4-ibcs-specific-usage" id="id-4-ibcs-specific-usage"></a>

_Note: To know the IBCS features and functionalities please refer to the_ [_IBCS user guide_](https://docs.vitaracharts.com/guideIBCSCommonFeatures/about.html)_._

To display certain details in the IBCS enabled chart, we can utilize the following macros in the text node chart together with the IBCS enabled Vitara chart. We require at least one IBCS enabled chart in the dossier/document to set IBCS macros in the text node chart. If the dossier contains multiple IBCS-enabled charts, we must select the chart on which we want to display the macro information. When you move your mouse over the chart, the “Edit” button will appear. When you click the “Edit” button, a popup window will appear. Select the chart to which you wish to apply the macro from the “Text Properties” menu’s “Select Chart Type” drop down box.

\


**&\[chart.list]:**

This macro lists the sub graphs used to display series data types in the selected chart.\
Data Types: Actual data (AC), Planned data (PL), Delta planned data, Percentage delta planned data.\
\


**&\[chart.count]:**

This macro will display number of sub graphs used in the IBCS mode.\
\


**&\[chart.dataTypes]:**

This macro will display the data types used in the chart: AC, PL, Delta PL, Percentage Delta PL.\
\


**&\[chart.sortBy]:**

This macro provides information about the series used to Sort the IBCS enabled chart.\
\


**&\[category.range]:**

This macro will list starting and ending element in the category axis and the series used to draw those category elements.\
\
