# Play Animation

The option ‘Play By First Attribute’ causes Vitara charts to display the chart for each element of the first attribute at a specific time instant. We can take a break at any time.

Note:To enable the ‘Play Animation’ option, at least two attributes must be present in the chart.

#### Steps to enable ‘Play Animation’ feature in dossiers: <a href="#steps-to-enable-play-animation-feature-in-dossiers" id="steps-to-enable-play-animation-feature-in-dossiers"></a>

Drag the ‘Play Axis’ attribute you want to apply into the ‘Play Axis’ drop zone.

Drag one of the attributes into the ‘Play Axis’ drop zone to enable the ‘Play Animation’ feature. In the above example, I used the month attribute as the play axis.

Click on play button to run the ‘Play Animation’ feature.

#### Steps to enable ‘Play Animation’ feature in report services documents: <a href="#steps-to-enable-play-animation-feature-in-report-services-documents" id="steps-to-enable-play-animation-feature-in-report-services-documents"></a>

**Step 1:**

Place all the attributes required in the grid. The attribute we want to place in the play axis should be the first attribute in the grid.

**Step 2:**

Run the document in presentation mode to display the chart.

**Step 3:**

Hover the pointer over the chart to reveal the ‘Edit’ button on the right side. Select the ‘Edit’ button. We have checked the box ‘Play by First Attribute’ in the ‘Appearance’ attribute. Check this box to enable play animation in the chart.

#### Customizing Play Animation <a href="#customizing-play-animation" id="customizing-play-animation"></a>

We can modify the speed of the play axis upto 0.5X, 1.0X, 1.5X,2.0X. If we want the play axis to play continuously, we can enable the Loop option.

Click on the settings button which is right edge of the play axis. Select the speed required.

**Retain Points**

From the 4.9.3 version, Retain point (First,Last but one) feature now moved under Play Axis tab which can be accessed from property editor window. When we select the ‘First’ option under retain point, the first elements are displayed in comparison to the final elements.\
The “Last but one” will similarly compare the final element with the play sequence’s last element.

This feature can be used to compare the trend in the play animation.

**The following vitara charts supports play animation feature:**

Bar chart, column chart, pie chart, line chart, area chart, bubble chart, tornado chart, spark line chart, funnel chart, column range chart, and bullet chart.

**The following charts don’t support play animation feature:**

Stacked bar/column, KPI Ring, heat map, waterfall, animation gauge, calendar heatmap, trellis, simple kpi, grid, micro, mekko, word cloud, waffle, histogram, slope chart, dumbbell, packed bubble, angular gauge, and sanky chart.
