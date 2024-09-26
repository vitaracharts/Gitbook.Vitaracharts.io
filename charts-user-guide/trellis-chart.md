# Trellis Chart

Please use the Small Multiples feature instead. Trellis chart will continue to work for existing use cases but will no longer be enhanced

The trellis chart shows a graph for each element of the first attribute. We can change the graph type to line or bar or column or scatter.

#### Inputs <a href="#inputs" id="inputs"></a>

Metrics: 1 metric Attributes: 2 attributes Use as Filter Option - Available

Option to set chart type - line, column, bar or scatter. We can set a number of columns to show the subgraph for each element of the first attribute.

#### Markers <a href="#markers" id="markers"></a>

Marker properties have been moved to Series properties in Vitara charts since version 4.6. The modified marker characteristics are used by all charts that support Series as Line/Area. By selecting the Series tab and clicking the ‘Edit’ button, you can see the Enable marker, Marker type, and Marker size options to Enable marker properties. There are numerous markers to choose from. Navigate to the marker tab, choose the marker type, and then select the marker. The size of the markings can also be changed. Simply type a number into the ‘Marker Size’ text input box, or use the increase/decrease buttons.

In the below example, the profit metric line changed to area in series property and ‘thanos.svg’custom marker is applied for the profit metric element. Below is the screenshot with the marker applied in the chart.

#### Series <a href="#series" id="series"></a>

We can turn the line/area chart into the combinational chart by changing the ‘series type’ in the ‘series’ tab.

From version 4.9.0, this charts have the Pattern fill option (Grid/Square/Double Square/Slash) in the Series tab, which allows us to display data in a more presentable manner.

#### Thresholds <a href="#thresholds" id="thresholds"></a>

In the business point of view, certain part of the chart needs to be highlighted to draw more attention from the desicion makers. For example, highlight the stores where total sales is greater than a specific value or highlight the top 10 products whose sales is high during last year’s winter. Thresholds are very useful objects in these use cases.

Thresholds will display some conditional formatting in a chart to highlight certain data points depending on predefined criteria.The criteria are attribute or metric qualifications. If a qualification’s expression evaluates to TRUE, the report displays the threshold. We can also include markers in thresholds.

To apply thresholds in vitara charts, hover the cursor on the chart. Vitara chart will display an ‘Edit’ button. When you click on this ‘Edit’ button the properties window will pop out. Select the thresholds tab to open threshold editor. In the window you can add a new threshold or delete any existing threshold or modify the existing threshold.

Note: From 4.6 version we can apply thresholds using attributes. The source drop down box in the threshold editor window will list all the attributes and metrics in the chart. we can select an attribute as source and define a threshold condition. The target of the threshold depends on the series of the chart. This means, if the chart series is created using metrics then target drop down box will display the metrics. If we enabled ‘color by’ mode, by adding an attribute to the ‘color by’ drop zone in the dossier’s editor panel, the chart series will be created using attributes. In this case the threshold target drop down box will show all the elements of attribute used in the color by drop zone. In this case we can set threshold target using attribute.

In the threshold editor window apply source, target, threshold condition and the other related information to set a threshold on the chart.

After giving all the inputs click on ‘Apply’ button.

From version 4.9.0, we can use pattern fill in thresholds, certain part of the chart can be filled with a pattern.

#### Background Image <a href="#background-image" id="background-image"></a>

The steps to set a background image for all Vitara charts are explained in backgroundImage.

#### Gradient Color <a href="#gradient-color" id="gradient-color"></a>

From version 5.0, Gradient color fill can be added where the series property is available.

It can be enabled by selecting options from the series tab for individual series.

It will show the color palette, which will have two selection handles to choose two colors that will render from beginning to end on the series. (From left to right)

#### Series based Tooltip and Datalabels <a href="#series-based-tooltip-and-datalabels" id="series-based-tooltip-and-datalabels"></a>

We introduced in version 5.2.4 ,the “Series-based Tooltip” and “Data Labels” features enhance chart data display. When you hover over a data series, series-based tooltips appear, revealing insights into individual data points. Data Labels, on the other hand, allow you to directly display data values on chart elements, which improves data comprehension. These characteristics are useful for expressing precise information and promoting a deeper comprehension of plotted data, making charts more informative and user-friendly.

This feature will be accessible from the “Series” tab in the chart editor menu. Users can access this tab when editing a bar/column chart. Within the “Series” tab, under the metrics two new option named “Data label and Tooltip “ is added, accompanied by a dropdown menu that allows users to select the desired formatting , by default it will be none.In the below screenshots ,I have made changes for the ‘Cost’ series.
