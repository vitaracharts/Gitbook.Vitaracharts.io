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

# Custom CSS

These features are supported in the release 4.2 (or newer)

**Important Note:** **After making any changes, you must clear your browser’s cache to ensure the updates are reflected in Vitara Charts.**

## Custom CSS in Vitara Charts <a href="#custom-css-in-vitara-charts" id="custom-css-in-vitara-charts"></a>

If you use custom CSS styles in Vitara Charts, no presentational characteristics (such as fill, stroke, font styles, and so on) are applied to the chart SVG. Instead, CSS is used to apply the design.

To customize your styles, edit the customStyles.css file and add your own CSS rules.

The customStyles.css file is located at,

```
tomcat/webapps/MicroStrategy/plugins/VitaraCharts/custom
```

The following is an overview of the CSS rules which are internally set on the VitaraCharts.

## CSS Rules <a href="#css-rules" id="css-rules"></a>

```
.vitara-chart-background
```

The chart area background. Use this to set the chart area background fills.

```
.vitara-plot-background
```

The plot area background. Use this to set the plot area background fills.

```
.vitara-category-axis
```

Class for the category axis. Use this to set the category axis labels text style.

```
.vitara-value-axis
```

Class for the value axis. Use this to set the value axis labels' text style.

```
.vitara-axis-title
```

The title of the axis. Set the axis title text style with this. To set the title of a given axis, use this class in conjunction with the category or value axis. Text characteristics such as font-family, font-style, color, text-decoration, text-transform, and letter-spacing can be changed.

```
.vitara-axis-line
```

The axis line is a straight line. Set the width and color of the axis line with this. To set the axis line attributes of a certain axis, use this class in conjunction with the category or value axis.

```
.vitara-line-display
```

The line series. Use this to set the default line style in any line series. Use this class in conjunction with the chart's class name to specifically set the line properties of that particular chart. Line properties like stroke-dasharray, stroke and stroke-width can be set.

```
.vitara-grid-line
```

The grid line. Use this to set the grid line properties. Line properties like stroke-dasharray, stroke and stroke-width can be set.

```
.vitara-legend-text
```

The legend item text. Use this to set the legend item text style. Can change text properties like font-family, font-style, color, text-decoration, text-transform, letter-spacing.

```
.vitara-marker
```

Can change the fills and strokes and sizes of markers on VitaraCharts selected from the Marker tab in the property editor.

```
.vitara-datalabel
```

The datalabel. Use this to change the text style of datalabels. Can change text properties like font-family, font-style, color, text-decoration, text-transform, letter-spacing.

```
.vitara-point
```

* The default class for any data element on the chart.
* For example, in bar chart a bar is a data element and in a bubble chart a bubble is a data element.
* Use this to change the text style of datalabels. Can change text properties like font-family, font-style, color, text-decoration, text-transform, letter-spacing.

\### CSS Class Names of charts | Chart Name | Class Name | | :--------------- | :------------------- | | Vitara Bar Chart | .VitaraHCBarChart | | Vitara Stacked Bar Chart | .VitaraHCStackedBarChart | | Vitara Column Chart | .VitaraHCColumnChart | | Vitara Stacked Column Chart | .VitaraHCStackedColumnChart | | Vitara Pie Chart | .VitaraHCPieChart | | Vitara KPI Ring Chart | .VitaraHCKPIRingChart | | Vitara Line Chart | .VitaraHCLineChart | | Vitara Area Chart | .VitaraHCAreaChart | | Vitara Bubble Chart | .VitaraHCBubbleChart | | Vitara Tornado Chart | .VitaraHCTornadoChart | | Vitara Sparkline Chart | .VitaraHCSparklineChart | | Vitara Heatmap Chart | .VitaraHCHeatmapChart | | Vitara Funnel Chart | .VitaraHCFunnelChart | | Vitara Column Range Chart | .VitaraHCColumnRangeChart | | Vitara Bullet Chart | .VitaraHCBulletChart | | Vitara Waterfall Chart | .VitaraHCWaterfallChart | | Vitara KPI Animation Chart | .VitaraKPIAnimationChart | | Vitara Calendar Heatmap | .VitaraD3CalHeatMapChart | | Vitara Simple KPI Chart | .VitaraSimpleKPIChart | | Vitara Mekko Chart | .VitaraMekkoChart | | Vitara Word Cloud | .VitaraHCWordCloud | | Vitara Waffle Chart | .VitaraD3WaffleChart | | Vitara Histogram Chart | .VitaraHistogramChart | | Vitara Dumbbell Chart | .VitaraHCDumbbellChart | | Vitara Slope Chart | .VitaraHCSlopeChart | | Vitara Circle Packing Chart | .VitaraD3CirclePackingChart | | Vitara Angular Gauge Chart | .VitaraHCAngularGaugeChart | | Vitara Sankey Chart | .VitaraHCSankeyChart | [View sample implementations](custom-css-samples.md)
