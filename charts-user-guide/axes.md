# Axes

\


### Category Axis <a href="#category-axis" id="category-axis"></a>

Under Category axis settings, we can format the axis labels, axis title, axis line, hide/unhide axis etc. Let’s see some of them

#### Enabling/Disabling attribute form name in axis labels <a href="#enablingdisabling-attribute-form-name-in-axis-labels" id="enablingdisabling-attribute-form-name-in-axis-labels"></a>

When we enable attribute forms for an attribute in the chart, then by default attribute form \[id in particular] will be enabled on the chart as well.\
In case if we want to turn off the attribute form for axis label, then disable ‘show attribute id’ checkbox in the property editor here: Axis > Category Axis > Label\
To know more about attribute forms in axis labels click [here](https://about/guideCommonFeatures/attributeForms.html#choose-specific-attribute-forms-to-display-on-the-chart)

#### Multi level Axis rotation <a href="#multi-level-axis-rotation" id="multi-level-axis-rotation"></a>

Starting with VitaraCharts 4.8, each level can independently rotate the labels on the category axis. This implies that when there are two attributes in the chart, we can individually control the rotation of each level’s axis label. Axis label rotation can also be configured independently for each level when there are 3 attributes. All charts that include horizontal category axis labels are capable of using this feature. Using the example below, let’s examine this. With two attributes \[Quarter, Month] and a measure, we have a column chart. View the resulting screenshot. See the screenshot below\


The category axis labels at two levels in the above screenshot were rotated to some value by default based on the available space. For each level, we are able to get the labels to spin at a distinct value. For instance, if level 1 = 0, level 2 = -90. Also, have a look at the graphic below to see how things have changed.&#x20;

And let’s say we have 3 attributes \[year, quarter, month]. We set the rotation for level 1 = -90, level 2 = -45, level 3 = 0. See the screenshot below\


### Value Axis <a href="#value-axis" id="value-axis"></a>

Under value axis settings also, we can format the axis labels, axis title, axis line, hide/unhide axis etc. Let’s see some of them

#### Use Metric Formatting. <a href="#use-metric-formatting" id="use-metric-formatting"></a>

Just like we have ‘use metric formatting’ option for data labels, there is an option added for value axis labels also. This option is available in **Axes > Value axis > Label** tab of the property editor. See the screenshot below\


This property is linked with the ‘metric format’ property available in data labels. That means, if you enable this property, the value axis labels take the formatting of the data labels.\
To understand this, let’s take an example of the below screenshot\


As you can see in the screenshot above, the datalabels and axis labels formats are distinct. If you want the same format for axis labels, click the ‘use metric formatting’ box under the value axis tab. The chart then appears as seen below. Take a look at the screenshot below.&#x20;

#### Tick interval <a href="#tick-interval" id="tick-interval"></a>

The ‘Tick interval’ setting is now available in the Axes tab as of version 4.3. This feature allows you to change the scale of the value axis. This option may be found in Axes > Value axis > Other. This option is available for both the major and secondary axes. See the image below.&#x20;

Let’s see this setting with the example below. We have a bar chart with 2 attributes and 2 metrics.\


In the following chart, the default tick interval is 2M (two millions). Now we’ll change the tick interval to 1M (one million). Simply enter ‘1000000’ in the tick interval textbox to achieve this. See the screenshot below for an updated tick interval on the chart.&#x20;

Setting up the tick interval for values in % format:\
Below is a column chart with metrics in percentage format.\


The default tick interval for the above chart is 10%. Now we will customize the tick interval to 5%. For this to happen, we have to put ‘0.05’ the tick interval textbox instead of ‘5%’\
See the below screenshot which shows the updated tick interval\


#### Start / End Values <a href="#start--end-values" id="start--end-values"></a>

The value axis can have start and end values set. A metric, fixed value, or percentile basis can be used to specify the start or end value. Axes > Value Axis > \[Start Value, End Value] provides access to these properties. View the property editor in the screenshot.&#x20;

Let us discuss start/end values with an example below\


All four bar values in the screenshot above are greater than 30.7% and less than 31.2%. Therefore, there is no advantage to the bars beginning at 0%. Therefore, the results may be properly examined if the start value is set to 30.7% (0.307) and the final value to 31.2% (0.312). View the screenshot to see the start and end values.&#x20;

And after specifying the start & end values, the chart looks like the below screenshot\


#### Sync Axis <a href="#sync-axis" id="sync-axis"></a>

From version 5.1 , The primary and secondary axes are now synchronized via a new feature that we have added. We must enable the secondary axis for one of the metrics under the series tab in order to enable the new feature.

The primary and secondary axes values are aligned in the screenshot below.

#### Truncating and Wrapping <a href="#truncating-and-wrapping" id="truncating-and-wrapping"></a>

From version 5.1, We have added new features to the label’s property that allow us to customize the labels by truncating or wrapping them.

Truncating

Wrapping

We can also control the labels from the value axis category in case of Bubble and Heatmap Charts.

#### Label interval <a href="#label-interval" id="label-interval"></a>

Version 5.2.8 introduces two significant enhancements in the Axes tab that allow for greater customization of the category axis:

1. Label Interval : This feature enables users to control the scale of their category axis by adjusting the interval between labels. This customization can help in optimizing the readability of charts with densely packed data points.
2. Label Start Index : This allows users to define the starting point for x-axis labels, giving them more control over how data is presented and enhancing the overall user experience.

Let’s delve into these new features and explore how they can elevate your user experience.This option is available in Axes > Category axis > Labels tab of the property editor. See the screenshot below:&#x20;

Here’s an example to illustrate the Label Interval and Label Start Index settings: We have a dataset with 200 data points, and want to ensure that the labels on the x-axis are clearly visible without overcrowding.

Example Settings:

1. Label Interval: Since we have 200 data points, a suitable label interval would be between 10-15. Setting the interval to 10 means that every 10th label on the x-axis will be displayed.
2. Label Start Index: If we set the Label Start Index to 5, the labels will start displaying from the 5th data point. With the interval set to 10, the labels would be displayed at data points 5, 15, 25, and so on. The x-axis would start showing labels from the 5th data point and continue at every 10th interval. This configuration ensures that the chart remains clear, and the labels are not overlapping, making it easier to interpret the data.

Refer to the screenshot below ,after applying the specified Label Interval and Label Start Index settings.&#x20;

#### Impact of Label Interval on Category Label Rendering in Charts <a href="#impact-of-label-interval-on-category-label-rendering-in-charts" id="impact-of-label-interval-on-category-label-rendering-in-charts"></a>

When visualizing large datasets with numerous categories (100+), setting an excessively small interval (e.g., 2 or 3) can lead to suboptimal label rendering. In such cases, Highcharts may struggle to fit all category labels within the chart area, resulting in overlapping labels.

To ensure clear and effective visualization, it’s recommended to adjust the label interval based on the dataset size. The relationship between the Label Interval and dataset size is linear, meaning that as the number of data points increases, the label interval should also increase to maintain chart clarity. For instance:

* Datasets with 100+ categories: Use a label interval of 5-10.
* Datasets with 200+ categories: Use a label interval of 10-15.
* Datasets with 300+ categories: Use a label interval of 15-20.and so on
