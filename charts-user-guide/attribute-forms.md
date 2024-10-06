# Attribute Forms

\


### Attribute forms in the Vitara Charts <a href="#attribute-forms-in-the-vitara-charts" id="attribute-forms-in-the-vitara-charts"></a>

Vitara charts supports multiple attribute forms.

#### Attribute forms in XY Charts: <a href="#attribute-forms-in-xy-charts" id="attribute-forms-in-xy-charts"></a>

\
For example, i want to show customer wise number of complaints or tickets raised and the complaints or tickets resolved. The customer attribute has two attribute forms _**First Name**_ and the _**Last Name**_. The chart has to show the complete name of the customer, which is the combination of both the attribute forms _**First Name**_ and the _**Last Name**_.

Attribute and Metrics used in this example are:\
Attributes: 1.Customer\
Metrics: 1.Tickets Raised 2.Tickets Resolved

Below is the screenshot of the MicroStrategy grid visualization. You can see, for the customer attribute both the attribute forms _**First Name**_ and the _**Last Name**_ are enabled.

If we convert this visualization into any of the vitara charts, vitara charts will concatinates both attribute forms and display as a single label. Below is is the screenshot of vitara combination chart with multiple attribute forms enabled for the customer attribute.

#### Choose specific attribute forms to display on the chart <a href="#choose-specific-attribute-forms-to-display-on-the-chart" id="choose-specific-attribute-forms-to-display-on-the-chart"></a>

From 4.4 version, an option ‘show attribute id’ is added in category axis label tab. By default, this option will be in enabled state. See the screenshot:\
\


This feature helps us to choose whether or not to display the attribute forms on the axis even if we enable attribute forms for the chart.\
For example, we have an attribute ‘category’ in a chart. Both attribute forms ‘ID’ and ‘DESC’ are enabled for the category attribute. Then both the attribute forms will be shown on the category axis. See the below screenshot.\
\


If we need the attribute forms to be enabled for the chart and not to display the forms on the axis, then we can disable them from the category axis menu. See the screenshot\
\


#### Attribute forms in Data labels and Tooltip <a href="#attribute-forms-in-data-labels-and-tooltip" id="attribute-forms-in-data-labels-and-tooltip"></a>

Attribute forms can also be used in data labels and tooltip\
To know more about attribute forms in data labels, go to [Data labels](https://about/guideCommonFeatures/datalabelCustomization.html#attribute-forms-in-data-labels)\
To know more about attribute forms in tooltip, go to [Tooltip](https://about/guideCommonFeatures/tooltipCustomization.html#attribute-forms-in-tooltip)\


#### Attribute forms in Grid and Micro Charts: <a href="#attribute-forms-in-grid-and-micro-charts" id="attribute-forms-in-grid-and-micro-charts"></a>

\
In the vitara grid and micro charts each attribute form is displayed as a separate column. Below is the sceenshot of the vitara grid chart showing the same example explained above.
