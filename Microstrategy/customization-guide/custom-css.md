# Custom CSS

These features are supported in the release 5.3.10 (or newer)

#### Important Note :&#x20;

* For versions **older than 5.3.10**, do NOT include the .vitara namespace.\
  The new .vitara prefix should be used **only from version 5.3.10 onward**

&#x20;**After making any changes, you must clear your browser’s cache to ensure the updates are reflected in Vitara Charts.**

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
.vitara .vitara-chart-background
```

The chart area background. Use this to set the chart area background fills.

```
.vitara .vitara-plot-background
```

The plot area background. Use this to set the plot area background fills.

<pre><code><strong>.vitara .vitara-category-axis
</strong></code></pre>

Class for the category axis. Use this to set the category axis labels text style.

```
.vitara .vitara-value-axis
```

Class for the value axis. Use this to set the value axis labels' text style.

```
.vitara .vitara-axis-title
```

The title of the axis. Set the axis title text style with this. To set the title of a given axis, use this class in conjunction with the category or value axis. Text characteristics such as font-family, font-style, color, text-decoration, text-transform, and letter-spacing can be changed.

```
.vitara .vitara-axis-line
```

The axis line is a straight line. Set the width and color of the axis line with this. To set the axis line attributes of a certain axis, use this class in conjunction with the category or value axis.

```
.vitara .vitara-line-display
```

The line series. Use this to set the default line style in any line series. Use this class in conjunction with the chart's class name to specifically set the line properties of that particular chart. Line properties like stroke-dasharray, stroke and stroke-width can be set.

```
.vitara .vitara-grid-line
```

The grid line. Use this to set the grid line properties. Line properties like stroke-dasharray, stroke and stroke-width can be set.

```
.vitara .vitara-legend-text
```

The legend item text. Use this to set the legend item text style. Can change text properties like font-family, font-style, color, text-decoration, text-transform, letter-spacing.

```
.vitara .vitara-marker
```

Can change the fills and strokes and sizes of markers on VitaraCharts selected from the Marker tab in the property editor.

```
.vitara .vitara-datalabel
```

The datalabel. Use this to change the text style of datalabels. Can change text properties like font-family, font-style, color, text-decoration, text-transform, letter-spacing.

```
.vitara .vitara-point
```

* The default class for any data element on the chart.
* For example, in bar chart a bar is a data element and in a bubble chart a bubble is a data element.
* Use this to change the text style of datalabels. Can change text properties like font-family, font-style, color, text-decoration, text-transform, and letter-spacing.

#### ### CSS Class Names of charts

| **Chart Name**               | **Class Name**                     |
| ---------------------------- | ---------------------------------- |
| Vitara Bar Chart             | .vitara.VitaraHCBarChart           |
| Vitara Stacked Bar Chart     | .vitara.VitaraHCStackedBarChart    |
| Vitara Column Chart          | .vitara.VitaraHCColumnChart        |
| Vitara Stacked Column Chart  | .vitara.VitaraHCStackedColumnChart |
| Vitara Pie Chart             | .vitara.VitaraHCPieChart           |
| Vitara KPI Ring Chart        | .vitara.VitaraHCKPIRingChart       |
| Vitara Line Chart            | .vitara.VitaraHCLineChart          |
| Vitara Area Chart            | .vitara.VitaraHCAreaChart          |
| Vitara Bubble Chart          | .vitara.VitaraHCBubbleChart        |
| Vitara Tornado Chart         | .vitara.VitaraHCTornadoChart       |
| Vitara Sparkline Chart       | .vitara.VitaraHCSparklineChart     |
| Vitara Heatmap Chart         | .vitara.VitaraHCHeatmapChart       |
| Vitara Funnel Chart          | .vitara.VitaraHCFunnelChart        |
| Vitara Column Range Chart    | .vitara.VitaraHCColumnRangeChart   |
| Vitara Bullet Chart          | .vitara.VitaraHCBulletChart        |
| Vitara Waterfall Chart       | .vitara.VitaraHCWaterfallChart     |
| Vitara KPI Animation Chart   | .vitara.VitaraD3KPIAnimationChart  |
| Vitara Calendar Heatmap      | .vitara.VitaraD3CalHeatMapChart    |
| Vitara Simple KPI Chart      | .vitara.VitaraSimpleKPIChart       |
| Vitara Mekko Chart           | .vitara.VitaraHCMekkoChart         |
| Vitara Word Cloud            | .vitara.VitaraHCWordCloud          |
| Vitara Waffle Chart          | .vitara.VitaraD3WaffleChart        |
| Vitara Histogram Chart       | .vitara.VitaraHCHistogramChart     |
| Vitara Dumbbell Chart        | .vitara.VitaraHCDumbbellChart      |
| Vitara Slope Chart           | .vitara.VitaraHCSlopeChart         |
| Vitara Circle Packing Chart  | .vitara.VitaraD3CirclePackingChart |
| Vitara Angular Gauge Chart   | .vitara.VitaraHCAngularGaugeChart  |
| Vitara Sankey Chart          | .vitara.VitaraHCSankeyChart        |

Click here to  [View sample implementations](custom-css-samples.md)
