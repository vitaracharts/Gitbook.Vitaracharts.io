# Variwide Chart

Convert a Column chart to a Variwide Column chart or a Bar chart to a Variwide Bar chart.

In a column chart, a variwide chart can be used to visualise a second dimension. In addition to its value, each data point is assigned a weight, which determines the breadth of the column. It computes the stack’s width to occupy the entire plot area and just allows the column widths to reflect a value.

Variwide charts can be created from column and bar charts. You must enable the Dynamic Width(metric\_name) to see the variwide chart. Variwide chart applications: Use the Vitara Column/Bar chart and navigate to the property editor. Property of an Open Column/Bar Enable the Dynamic Width (metric name) feature.

Below is the Variwide column chart where the Y-Axis represents the cost of the categories, while the column width is proportional to the categories.

Below is the Variwide Bar chart where the X-Axis represents the cost of the categories, while the column width is proportional to the categories.

**Axis formattings in variwide chart**

In a Variwide chart, the axis representing categories changes depending on the width of the stack to fill the entire plot space. The percentage of elements is determined as \[(value of datapoint/sum of all metric values) \* 100]. The screenshot below shows how the percentage of profit is determined in the variwide chart.
