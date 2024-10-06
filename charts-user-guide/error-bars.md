# Error Bars

This feature are supported in the release 4.3 (or newer)

Error bars are a graphical representation of the variability of data and are used on graphs to indicate the error, or uncertainty in a reported measurement. Currently, Vitara charts supports error bars in the following charts.

1. Vitara Bar Chart
2. Vitara Column Chart
3. Vitara Line Chart
4. Vitara Sparkline Chart

### How to set error bars in the vitara charts. <a href="#how-to-set-error-bars-in-the-vitara-charts" id="how-to-set-error-bars-in-the-vitara-charts"></a>

To set error bars in vitara charts, we need three metrics. One is the basis measure for which the error bars are calculated. ‘Error-Low Value’ and ‘Error-High Value’ are the other two measures.

#### Example: <a href="#example" id="example"></a>

Consider the following example: the open and closing values of the Amazon.com, Inc. stock price for the month of November 2019. I’d want to show the day’s high and low values as error bars on the close value measure. The following attributes and metrics are utilised in the example:

**Attributes:** 1.Date

**Metrics:** 1.Open ($), 2.Close ($), 3.Day High ($), 4.Day Low ($).

**Step 1:**

Insert a Vitara bar/column/line chart into a dossier/document. I utilized a Vitara column chart in this instance. Initially, I added metrics for Open ($) and Close ($) to the Vitara column chart.

I’d like to display the error bars on the **Close ($)** metric’s bars. Insert the Day High ($) and Day Low ($) metrics into the **Tooltip** dropzone. The metric **Day Low** ($) should be set as the error bar’s low value, and the metric **Day High** ($) should be set as the error bar’s high value.

**Step 2:**

To reveal the Edit button, move the cursor over the Vitara chart. To access the properties pane, click on the Edit button. Open the Series menu in the properties pane.

In basic terms, the series properties will be set up via the Series menu. This indicates the type of chart used to draw the series, the color of the series, and the axis for this series—primary/secondary—for a certain metric.

Edit the series properties for the measure for which you want to configure the error bars in the Series menu. For the metric Close ($) in the present example, click Edit.

**Step 3:**

In the series properties there is a check box **Show Error Bars**. Click on this check box to enable **Error Bars** in the chart.

**Step 4:**

When error bars are enabled, the drop-down list boxes to set low and high values for error bars appear in the series properties menu. Select the measurements you wish to designate as low and high values by expanding the drop-down list. then decide on the error bar’s color. Finally, press the Apply button.

Below is the screenshot of Vitara colum chart showing error bars on the metric **Close ($)**.

For the same example, below is the screenshot of the vitara line chart showing error bars.
