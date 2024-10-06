# Tooltip Customization

\


#### Introduction <a href="#introduction" id="introduction"></a>

Starting with the 3.9 release, we can customise what appears in the VitaraCharts tooltip. To edit tooltips, utilise the new HTML editor in the “Tooltip” property menu. The tooltip editing window is seen in the screenshot below.

The editor is a lightweight component that supports the following features:

Alignment (Right, Center, Left and Justify)

Font Style (Family, Size, Bold, Italic, Underline, Color)

Recognizing new lines

Markers

Support for macros (described below)

#### Macro Support: <a href="#macro-support" id="macro-support"></a>

The macro suggestion box is seen in the screenshot below. Hover the pointer over the ‘i’ sign to see the chart’s available macros.

The new tooltip editor component will give all possible element names that should be supported as macros (through invocation configuration options). For example, if a report has attributes Country, Category, and Sales, Profit Margin, then all of the following macros are possible in the tooltip editor:

Country

Category

Profit Margin

Sales

Metric Names

Metric Values

Attribute Values

When a user starts typing “&” character, all the possible macro suggestions will be shown.

When one of the macro elements is selected, the editor inserts it into the text (and saves it in the state) as &\[macroname].

So, if the user selects ‘Metric Names,’ the displayed macro will be &\[Metric Names].

The tooltip’s width is fixed at 30px. As needed, the height will increase. There are certain unique macros, such as ‘Metric Names,’ ‘Metric Values,’ and ‘Attribute Values.’

Typical syntax is: &\[Metric Names]: &\[Metric Values] or &\[Metric Names] = &\[Metric Values]

We go over all of the metrics (including those in the tooltip and data zones) and provide them in the desired way here.

As the name implies, the ‘Attribute Values’ macro contains the attribute elements (comma separated) at which the data point is assessed. For example, if a data point has Country=USA and Category=Electronics, the ‘Attribute Values’ macro will replace it with USA, Electronics.

#### Attribute forms in Tooltip <a href="#attribute-forms-in-tooltip" id="attribute-forms-in-tooltip"></a>

We can opt to display the macros for all attribute forms for all attributes in the tooltip.

For example, there are two attributes with attribute forms: ‘category’ and’subcategory’. Then, in tooltip macros, we may select macros for both attributes’ attribute forms. Take a look at the screenshot.&#x20;
