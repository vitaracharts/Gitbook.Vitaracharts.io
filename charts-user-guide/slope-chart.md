# Slope Chart

The slope graph depicts the change in metric value for a particular attribute value over time. As a result, each (sloping) line is represented by two points, one at the beginning and one at the end of time. When more than two time values are specified, all points are plotted in a line chart fashion. Along the slope-line connecting the points, a label displaying the percentage variation between two successive points is presented (optional).

#### Inputs <a href="#inputs" id="inputs"></a>

Metrics: 1 metric.

Attributes: 2 attributes.

One attribute must be the time that is plotted along the x-axis. The second attribute is used to categorize input data.

Use as Filter Option - Available

#### Data labels <a href="#data-labels" id="data-labels"></a>

We can format the data label and variation. You can see the attached screenshots below.

We have an option to enable/disable the All, Value and Variation Data labels.

**Labels inside the Marker**

We can now display data labels inside the marker starting with version 5.2. A slope chart’s readability and clarity can be improved by adding labels inside the markers by directly connecting the values to the corresponding data points. Viewers can more easily recognize and relate data points to their relevant categories by using labels inside markers. This is particularly helpful in slope charts, where the comparison of changes between two points for various categories is the main focus. This functionality can be enabled by going to the editor’s data labels property and checking the “Label inside the marker” check box.

#### Line Width and Line Style <a href="#line-width-and-line-style" id="line-width-and-line-style"></a>

With version 5.2, a new tab called ‘Slope’ was added, allowing us to customize the line style and line width. Line width can be used to highlight a trend or change in value for specific categories. If certain categories are more significant or demand extra attention, using a different line width for those categories can make them stand out. Different line types, such as solid, dashed, or dotted lines, can be used to differentiate between the slope chart’s many categories. This is particularly effective when numerous lines connect various categories, making it easier for viewers to distinguish between them. When comparing two conditions, time periods, or groups, utilizing various line styles for each set of data can help highlight the differences.

#### Thresholds <a href="#thresholds" id="thresholds"></a>

In the business point of view, certain part of the chart needs to be highlighted to draw more attention from the desicion makers. For example, highlight the stores where total sales is greater than a specific value or highlight the top 10 products whose sales is high during last year’s winter. Thresholds are very useful objects in these use cases.

Thresholds will display some conditional formatting in a chart to highlight certain data points depending on predefined criteria.The criteria are attribute or metric qualifications. If a qualification’s expression evaluates to TRUE, the report displays the threshold. We can also include markers in thresholds.

To apply thresholds in vitara charts, hover the cursor on the chart. Vitara chart will display an ‘Edit’ button. When you click on this ‘Edit’ button the properties window will pop out. Select the thresholds tab to open threshold editor. In the window you can add a new threshold or delete any existing threshold or modify the existing threshold.

Note: As of version 4.6, we can use characteristics to impose thresholds. All the measurements and attributes in the chart are listed in the source drop-down box in the threshold editing window. We can choose a source attribute and specify a threshold condition. The series of the chart determines the threshold’s aim. This indicates that the metrics will be displayed in the target drop-down box if the chart series was generated using metrics. The chart series will be constructed using attributes if “colour by” mode is enabled by adding an attribute to the “colour by” drop zone in the dossier’s editor panel. In this instance, all the attribute elements used in the colour by drop zone are displayed in the threshold target drop down box. In this case we can set threshold target using attribute.

In the threshold editor window apply source, target, threshold condition and the other related information to set a threshold on the chart.

After giving all inputs click on ‘Apply’ button.

From version 4.9.0, we can use pattern fill in thresholds (Grid/Square/Double Square/Slash), certain part of the chart can be filled with a pattern.

#### Markers <a href="#markers" id="markers"></a>

At the starting value point and ending value point, the marker is displayed. These markers type and size are customizable.

The marker feature in a slope chart is employed to highlight specific data points, making them easily identifiable within the chart. It aids in emphasizing critical events, such as turning points or anomalies, in data trends. For instance, markers can be used to pinpoint the exact date when a product’s sales dramatically increased. This feature enhances the chart’s clarity, helping viewers focus on essential data points and facilitating trend analysis, making it particularly useful in fields like finance, economics, and project management.

#### Plot lines / Reference Lines <a href="#plot-lines--reference-lines" id="plot-lines--reference-lines"></a>

We can set reference lines in slope chart. The steps to set plot lines /reference lines are explained in plotlines

#### Background Image <a href="#background-image" id="background-image"></a>

The steps to set a background image for all Vitara charts are explained in backgroundImage.

#### Small Multiples <a href="#small-multiples" id="small-multiples"></a>

Slope chart supports small multiples feature. Small multiples is explained in smallMultiples.
