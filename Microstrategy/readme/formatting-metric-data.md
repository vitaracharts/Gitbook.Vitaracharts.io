# Formatting metric data

* Use the _**Number Format**_ option under the right click menu on a metric name (from the dossier’s dataset panel) to define the desired format.
* All formats available under the _**Number Format**_ menu are supported (except aggregated values are not formatted in fraction)
* Red color coding for negative numbers is not supported (in any format). But use of minus (-) sign or parentheses () is retained in the vitara charts.

<figure><img src="../.gitbook/assets/formatting_Metric_Data_1.png" alt=""><figcaption></figcaption></figure>



## Usage of Metric Formatting: <a href="#usage-of-metric-formatting" id="usage-of-metric-formatting"></a>

There are two types of numbers in Vitara Charts

### **Actual data numbers**

* These numbers have a formatted value as defined by the users in the dataset.
* The actual data numbers are used in data labels and tooltips.

### **Aggregated numbers**

* These figures are the outcome of various aggregations conducted in Vitaracharts. (For example, axis labels, stack totals, and data values in charts such as Calendar Heat Map where the data is provided at the day level but graphically represented at a higher level such as week, month, or year)
* The formatted value of an Actual data number or format string from metric information is used to identify metric Format for these numbers.
* The identified metric format is used to format the aggregated value.
* Fractional formatting is not supported.

<figure><img src="../.gitbook/assets/formatting_Metric_Data_2.png" alt=""><figcaption></figcaption></figure>

## Vitara charts Identifying Metric Format: <a href="#vitara-charts-identifying-metric-format" id="vitara-charts-identifying-metric-format"></a>

Microstrategy delivers metrics with metadata that includes the format string and metric type.

The metric type is used to identify data values such as dates and percentages. Condensed format is identified via the Format string. Currency prefixes and suffixes (such as $/€). When the number format is set to automatic or custom, the date, scientific, and percentage metric types are displayed. In negative values, the following format is used: a minus symbol ‘-‘ or a pair of parenthesis ‘()’

## Percentage Format <a href="#percentage-format" id="percentage-format"></a>

**Existing Functionality:** MicroStrategy format string is used to identify percentage data. This is done regardless of the number format chosen in Microstrategy. When the % format string is specified, all data from the metric is assumed to be in percentage form. Aggregations made to metric data (through VitaraCharts menus) are updated as needed. All labels (data labels, axis labels, totals) and tooltips are properly formatted. Vitara Bar Chart Formatting (Formatted Values are shown in Microstrategy Grid Chart):&#x20;

<figure><img src="../.gitbook/assets/formatting_Metric_Data_6 (1).png" alt=""><figcaption></figcaption></figure>



* Using custom format in the same dossier:

<figure><img src="../.gitbook/assets/formatting_Metric_Data_4 (1).png" alt=""><figcaption></figcaption></figure>

* Using percentage format in the same dossier:

<figure><img src="../.gitbook/assets/formatting_Metric_Data_5 (1).png" alt=""><figcaption></figcaption></figure>

In all of the above instances, regardless of the metric’s Number Format, a formatted number (as seen in the Grid Chart) is utilised to denote the percentage data. Metric values are expressed as percentages in Data labels, Axis labels, and Tooltips.



## **Limitation:**

* If the formatted string contains ‘%’ symbol, the metric is identified to contain percentage data.\
  **Dossier with ‘%’ symbol in formatted string:**

<figure><img src="../.gitbook/assets/formatting_Metric_Data_6 (2).png" alt=""><figcaption></figcaption></figure>

In all the above screenshot, Formatted value(as shown in Grid Chart) shows ‘%’ even though the data is not in percentage form. Metric values in Data labels, Axis labels and Tooltips are incorrectly formatted as percentage.

## Time Formatting&#x20;

Starting from version **5.3.10**, VitarCharts supports **Time Metrics.**\
Metrics which represent  durations stored in seconds, minutes, milliseconds, or fractional days to be formatted and displayed as time values.

#### How to Apply

1. In the dossier’s Dataset Panel, right-click the metric name.
2. Select **Number Format**.
3. Choose a Time format (such as hh:mm, hh:mm:ss, mm:ss, etc.) based on your display requirements.\
   \
   ![](<../.gitbook/assets/unknown (8).png>)

**Examples:**

* A value like **0.31** is interpreted as a fraction of a day and formatted as **07:26**.
* A value like **95** (seconds) is displayed as **01:35** when using the mm:ss format.<br>

By default, Vitara Charts will reflect the applied Time Format. If the expected Number Format is not displayed, the user must select Use Metric Formatting from the Data Labels and Axis Labels tab the user must select Use Metric Formatting from the Data Labels and Axis Labels tab.

![](<../.gitbook/assets/unknown (19).png>)

&#x20;Once enabled, all chart elements—including data labels, axis labels, totals, subtotals, and tooltips—automatically adopt the applied time format and are displayed in the same format as defined in MicroStrategy.

#### Reference Screenshot

![](<../.gitbook/assets/unknown (9).png>)

After applying time format below is the screeenshot

![](<../.gitbook/assets/unknown (10).png>)

<br>
