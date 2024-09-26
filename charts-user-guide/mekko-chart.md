# Mekko Chart

The Mekko chart uses a two-dimensional axis to display data. It is comparable to a stack bar chart, but it also displays, by changing the width of the bars, how the various stack categories relate to one another. This will make it easier to determine how a given category contributed.

#### Inputs <a href="#inputs" id="inputs"></a>

Metrics: 1 metric

Attributes: 2 attributes.

Use as Filter Option - Available

Example: Mekko chart with Sales by Customer Segment & Province values. The width of each Customer Segment will represent the contribution of that Province to overall sales.

#### \&point.percentage macro <a href="#pointpercentage-macro" id="pointpercentage-macro"></a>

We now have the ability to incorporate a new macro in version 5.2 that displays the % value of the specified category as well as the overall percentage of the specific element in that chart.

To use this feature head to the data labels tab and from there in the text box field add \&point.percentage macro and apply the changes to the chart.

#### Thresholds <a href="#thresholds" id="thresholds"></a>

In the business point of view, certain part of the chart needs to be highlighted to draw more attention from the desicion makers. For example, highlight the stores where total sales is greater than a specific value or highlight the top 10 products whose sales is high during last year’s winter. Thresholds are very useful objects in these use cases.

Thresholds will display some conditional formatting in a chart to highlight certain data points depending on predefined criteria.The criteria are attribute or metric qualifications. If a qualification’s expression evaluates to TRUE, the report displays the threshold. We can also include markers in thresholds.

To apply thresholds in vitara charts, hover the cursor on the chart. Vitara chart will display an ‘Edit’ button. When you click on this ‘Edit’ button the properties window will pop out. Select the thresholds tab to open threshold editor. In the window you can add a new threshold or delete any existing threshold or modify the existing threshold.

Note: We can now apply thresholds using characteristics as of version 4.6. The source drop-down box in the threshold editing window contains a list of all the measurements and characteristics in the chart. We have the option of selecting a source property and a threshold condition. The goal of the threshold is determined by the chart’s series. This specifies that if the chart series was created using metrics, the metrics will be shown in the target drop-down box. If “colour by” mode is activated by adding an attribute to the “colour by” drop zone in the dossier’s editor panel, the chart series will be built using attributes. In this case, the threshold target drop-down box shows all the attribute items that were utilised in the colour by drop zone. In this case we can set threshold target using attribute.

In the threshold editor window apply source, target, threshold condition and the other related information to set a threshold on the chart.

Finally click on ‘Apply’ button.

#### Background Image <a href="#background-image" id="background-image"></a>

The steps to set a background image for all Vitara charts are explained in backgroundImage.
