---
description: Here's the list of all changes in each release (latest release first)
---

# Release Notes

### 5.3.2

* Improvement - Support Multiple Metrics in Funnel Chart.
* Improvement - Flexible Metric Selection for Value Axis Label Formatting.
* Improvement - revert to default Colour Customization in Data labels  macros.
* BugFix - GRID /Customer issue/Error Message in Vitara Grid Chart with Time Month Filte .
* BugFix - Customer issue- Column range doesn’t work with start/ end metric values.
* BugFix - MSTR(Customer Reported Issue): Arabic axis labels.
* BugFix - Grid chart : Right-click menu now have option for the contextual link.
* BugFix - Grid (MSTR) :Information window and target filter doesn't work when row grouped & drop zone attributes don't follow the same order.
* BugFix - Customer Reported Issue : Export from library shows error on last page.

### 5.3.1



* Bug Fix - Edit button Issue in MicroStrategy Library: The edit button was not showing up in the edit mode in Library. This was only an issue while working with the latest Sept 2024 release of MicroStrategy. This has now been fixed

### **5.3.0**

* Enhancement - Vitara KPI Animation Chart.
* Enhancement - Grid : Ability to hide the pivot column groups totals while column totals are enabled.
* Enhancement - Feature enhancement in Line chart visualization (X- axis Label interval).
* Enhancement - Show Pivot Metric Totals' has been renamed to 'Pivot Group Metric Totals' for improved clarity.
* Bug Fix - Customer Reported Issue: Overlapping data labels in Waterfall graphs.
* Bug Fix - Customer Reported Issue:Data Label Shift After Release.
* Bug Fix - Customer Reported Issue: Issues with Thresholds Vitara Line Chart.
* Bug Fix - Customer Reported Issue:Vitara Column Charts with IBCS - missing options.
* Bug Fix - Customer Reported Issue:Export to pdf : While exporting “Vitara Text” – the page in the dashboard to PDF an error appears.
* Bug Fix - Customer Reported Issue:Overlapping data labels in Waterfall graphs.
* Bug Fix - Customer Reported Issue:Not able to rename the header of the group in Non -English Locale.
* Bug Fix - Customer Reported Issue:If we apply column Grouping, then color are not changing for horizontal bars.
* Bug Fix - Customer Reported Issue:Ipad (Pie Chart) : If we enable "show Total in center label " and apply Element/Value Filter ,then total in center lable is not working according to the filter.
* Bug Fix - Customer Reported Issue:Waterfall Chart : Category Axis Label Shift After Release.
* Bug Fix - Customer Reported Issue:The marker icon in the legend shows a line at the center of the marker.

### **5.2.7**



* Enhancement - Stacked Bar Chart: Increase Bar Width limit
* Enhancement - New Macros for Sankey Chart Tooltips: node.source and node.target
* BugFix - Waterfall chart : Decimals not showing on mobile iOS/iPadOS.(Locale)
* BugFix - Customer Issue: sorting percentages
* BugFix - Grid chart : The tooltip takes a few seconds to appear when you hover the mouse over.
* BugFix - Issue regarding target visualization not working for Vitara Sankey Plot
* BugFix - Tooltip not showing attributes values of all source nodes in Vitara Sankey Chart.
* BugFix - Calendar Heat Map is not working in hungarian locale.
* BugFix - Customer Issue: Information Window tooltip and vitara line chart tooltip overlapping
* BugFix - Backward Compatibility : Category Axis Label Alignment in Bar chart.
* BugFix - Value axis not showing correct format in swiss user.
* BugFix - Custom SVG Marker from URLs not working in Web.
* BugFix - Bubble size is not identified in Non-English locales.

### **5.2.6**



* Enhancement - New DataLabels Option for Waterfall Chart: Display Negative Values Below, Positive Values Above Bars.
* Enhancement- Sankey Chart Update: Negative Values Supported with Red-Colored Nodes and Links.
* Enhancement- Enhanced Pivot Display(GRID): Toggle 'Show Pivot Metric Totals' for Detailed Totals on Expanded Groups.
* Bug Fix- Security vulnerability in common-codec 1.13.jar.
* Bug Fix- Heatmap sorting columns and rows problem.
* Bug Fix- Data Label Visibility Issue in MicroStrategy Column Chart with Absolute/Relative Variance.
* Bug Fix- Heat Map Totals Displaying Incorrect Values with Numeric Data in Attributes.
* Bug Fix- IBCS: Enable/disable labels on a specific series.
* Bug Fix- Tooltip text is not visible after upgrading to 4.9.3 from 4.0.1.
* Bug Fix- Stacked Bar Chart : Legend On-Off Functionality.
* Bug Fix- Small Multiple Chart Title and Bar value are overlapping each other.
* Bug Fix- Microsoft Sans Serif font in Vitara visualizations - do not correspond to the actual appearance of the specified fonts.
* Bug Fix- CSS from third party plugins overriding vitara elements.
* Bug Fix- Disabled Auto Scroll Functionality in Export Feature.
* Bug Fix- All chart : Font Family with numeric string was not working.

### **5.2.5**



* Enhancement -Bar/column: Possibility to remove spaces between the columns.
* Enhancement- Support for scrollable charts
* Enhancement- Grid Chart: Ability to group metrics in metric to row setup
* Enhancement - Null points : Need an option to connect null value points.
* Enhancement-Ability to apply thresholds when metric (or attribute) pivoting is applied.
* Bug Fix- Once the 'show bar for zero value' option is enabled and disabled the chart shows bars for zero values all the time
* BugFix- Datamarkers update
* Bug Fix- Vitara Gauge not shown correctly after Update to MSTR 2021 U11
* Bug Fix- Waterfall : Data Labels are cutting off on top of bars.
* Bug Fix- Can't disable tooltip in our Vitara KPI widget
* Bug Fix- Stacked Bar Chart : Legend On-Off Functionality.
* Bug Fix-Line Chart : Vitara Legend on-off functionality
* Bug Fix-Grid chart : subtotals (“Total” column) are not shown anymore in locale.

### **5.2.4**



* New Feature: Show aggregate and show top category options in bar and column charts.
* New Feature: Bubble chart: Ability to draw plotlines at some angle from 0 axes.
* New Feature: Play axis option to the stacked bar and stacked column charts.
* New Feature: Series-based tooltips and data labels for bar, column, stacked bar/column, line, area, and tornado charts.
* New Feature: Stacked Chart: Ability to re-order or reverse legend items.
* New Feature: Reference Line feature in the KPI Ring chart.
* Improvement: Calander heatmap will display filtered cells only instead of the entire month; eliminate the gray cells.
* Improvement: Bubble chart: In the bubble tab, we added an option to change the marker type for the entire chart.
* Improvement: Bubble chart: In scatter chart mode, option to customize the size of the bubbles.
* Bug fix: Vitara grid is not transparent despite setting it at the dossier level.
* Bug fix: Grid Chart: When the threshold source and target are the same and applied specifically to the year it doesn't get applied.
* Bug fix: Bubble Chart shows an error when dropping any random attribute into the category axis.
* Bug fix: Data labels are cut off in cases where values are closer to the visualization border.
* Bug fix: Dumbbell chart: Ability to customize the percentage data labels.
* Bug fix: Text Chart: Null attribute elements display the name of the macro.
* Bug fix: IBCS error when the charts have outliers in relative variance.
* Bug fix: Missing labels for KPI Ring and column Charts when upgraded from version 4.9.3

### **5.2.3**



* Bug fix: Fixed some security vulnerabilities related to resource loading.

### **5.2.2**



* Bug fix: Grid chart Localization: When row groups are enabled, in non-english locales the elements are incorrectly shown using just macro names.

### **5.2.1**



* Improvement: IBCS Mode: The positioning of the data labels is updated so they don’t overlap.
* Bug fix: Grid Chart: When metrics are moved to rows, the hide, pin column, and pivot functionalities disappear from the chart.
* Bug fix: Grid Chart: When attributes are grouped and subsequently metrics are moved to rows, the grouping is lost.
* Bug fix: Grid Chart: In a pivoted chart, when we move metrics to Rows, metrics are moved to rows and grouped accordingly, but the pivot is lost.
* Bug fix: Grid Chart: The shift metrics to rows operation returns the chart to its prior state, for example (grouping, pivot).

### **5.2.0** <a href="#user-content-5.2" id="user-content-5.2"></a>



* Enhancement: Grid chart: A custom editor was added to format cell data and headers. All the column formatting options are available in the new editor. To open this editor window, CTRL + click on the column header (meta + click on Mac) or choose "Format" from the hamburger menu of the column on the grid.
* Enhancement: Grid chart: The UI of the following components is redesigned: Column grouping menu, Trendline options menu, and Custom marker menu.
* Enhancement: The charts look is redesigned in Polar mode. The following charts will appear in the new design when polar mode is enabled: Bar, Column, Stacked bar, and Stacked Column.
* Enhancement: Sankey chart: Added options to set NodePadding, NodeWidth, and NodeOffsets in the editor menu. The NodeOffset option is used to move the nodes vertically and horizontally. The positive value moves it to the right/bottom, and the negative value moves it to the left/top. The NodePadding option can be used to increase/decrease the vertical spacing between the nodes and links.
* Improvement: In the Slope chart, added the ability to adjust the line width.
* Improvement: Added secondary delta options to IBCS Features in the Bar chart.
* Improvement: Data labels need to be shown inside markers in the Slope chart and dumbbell chart.
* Bug fix: Column chart: Data markers do not appear on the bars.
* Bug fix: Bar Show / Hide functionality not working as expected after clicking on Legends.
* Bug fix: Pie chart: The Show Overlapping Labels option does not force all the data to be visible on the chart.
* Bug fix: Maximum call stack size exceeded in Waterfall, Bullet, and KPI Animation charts.
* Bug fix: Grid chart: MicroStrategy number formatting is not applying on the labels of horizontal bars/pins.
* Bug fix: Text node chart: The chart is not displaying several elements.
* Bug fix: The size of data markers changed after the upgrade to 5.1.3 from 4.5.5.

### **5.1.6**



* Bug fix: Filter functionality is not working in the calendar heatmap.

### **5.1.5**



* Bug fix: Tooltip doesn't show fully for Calander Heatmap chart, Packed Bubble chart, and Waffle chart when we run dossiers in freeForm layout mode.

### **5.1.4**



* Bug fix: Improved rendering sequence for the charts to appear as soon as they are available, minimizing white screen time for a better user experience, especially when a large number of charts are rendered in a dossier/document.
* Bug fix: VitaraCharts Editor button is not enabled when using MSTR Workstation in connected mode.
* Bug fix: Changes to external files (global.txt, IBCSGlobal.txt, custom data markers) are not loaded when using MSTR Workstation in connected mode.\
  \[Workstation known issues in 5.1.4.047 version]\(\{{ site.data.navigation.allChartsDirectory \}}/workstationKnownIssues.html).

### **5.1.3**



* Enhancement: In the global.tx file, added a property to allow/block URLs using anchor tags in the data. _**security.allowURLLinks**_ = 0 or 1, setting 0 (zero) will not allow URLs used within the anchor tag “href” property. While setting to value 1 (one) will enable URLs used within the anchor tag href property.
* Enhancement: Added a new tab, Security, in the property editor. The option in this tab "Allow URL Links" can be used to enable URLs for specific dossier/RSD documents.
* Enhancement: The default sanitization for anchor tags is to remove all attributes and properties except title and inner content.
* Enhancement: Updated data sanitization rules specific to URLs (anchor tags), enabled strict check for URLs in all cases by default (for example: when data types are defined, link/html data was exempted until now).
* Bug fix: Fixed an error (unrecognized expression) in RSD documents with urls/html anchor tags present in the data.
* Bug fix: Fixed an error (unrecognized expression) in dossiers when using urls & “Create Links” option under Mstr data set options.

### **5.1.2**



* New Feature: Filter Chart.
* Enhancement: Tooltip feature in the simple KPI chart.
* Enhancement: Grid chart: - Ability to apply a threshold on the 'Grand Totals' row.
* Bug fix: Stopped printing unwanted error/warning messages to the console in.jsp files.
* Bug fix: Grid chart: The Formatting of labels displayed on horizontal bars/pins doesn't work.
* Bug fix: Grid chart: Currently, for 'horizontal Bars/Pins' as the trend line, we don't have the option to display the same scale for all group levels.
* Bug fix: Grid chart: In the presentation mode the right-click menu has a 'Show/Hide' grouping and pivot drop zones option which has no response when we use it.
* Bug fix: Grid chart: Datalabel alignment for Horizontal Bar/Pins is incorrect for negative and positive data.
* Bug fix: Rounding issue for percentage values in the waterfall chart.
* Bug fix: Pie chart: By default, chart display overlapping labels without enabling the show overlapping labels option.
* Bug fix: Tooltip position is not proper in the Simple KPI Chart.
* Bug fix: The background of the Simple KPI chart's tooltip is not working properly.
* Bug fix: Vitaracharts showing an error message: - Cannot read properties of undefined (reading 'formatted').
* Bug fix: HTML tags in the dataset in the tornado chart show mix metric formatting.

### **5.1.1**



* Improvement: Data Markers on Bars & Columns.
* Improvement: Hexagon bubble type for packed bubble chart.
* Improvement: Show bar for zero value is added to all charts that support bars.
* Improvement: In the pie chart, added the option "Show Overlapping Labels" in the data labels menu.
* Bug fix: The gradient threshold editor's 'customize stops' menu is not saving its state.
* Bug fix: Threshold input value issue for Gauge and KPI Animation charts with percentage metric.
* Bug fix: Decimal values on KPI animation threshold with percentage metric
* Bug fix: Consistency between entering the input percentage value for plotline and threshold.
* Bug fix: Bullet chart: Grammatical corrections in the new bands' editor window.
* Bug fix: Bullet chart: If we delete all the default bands, the editor window is not responding to creating a new band.
* Bug fix: If we use the HTML tag attribute in the drill target drop-down, the chart gets an error.
* Bug fix: Grid chart: If we move metrics to rows, the year column appears as "object object."
* Bug fix: Packed Bubble: Zooming on one visualization affects the second visualization, which hides data labels.
* Bug fix: Sparkline Chart: 0's are not aligned when used with small multiples.
* Bug fix: Sync primary and secondary axis labels: With some data, the 0-axis line collides with the next axis label.
* Bug fix: Pie chart: When we apply the same series pattern to different series, the color changes without being altered.

### **5.1.0** <a href="#user-content-5.1" id="user-content-5.1"></a>



* Improvement: Feature to adjust transparency in the color picker.
* Improvement: Customization of bands in the bullet chart.
* Improvement: Calendar heatmap will show year of the months in the header labels.
* Improvement: Localization of menu elements in calendar heatmap.
* Improvement: Pie chart now supports pattern fill feature.
* Improvement: Grid Chart: Added Filter in the group column hamburger menu.
* Improvement: Ability to select truncate or wrap the axis labels.
* Bug fix: Pattern fill isn’t working in polar mode.
* Bug fix: Use as filter (Filter target): When we use Data marker on the chart, use as filter (filter target) is not working when we click on the data markers.
* Bug fix: When we try to turning on the bar fill feature, dynamic width and overlay bar/column should be disabled.
* Bug fix: The order sequence of elements in Grouped Attribute is different in the chart than in group editor.
* Bug fix: Pattern fill option for thresholds is not available.
* Bug fix: When we apply series pattern, legends don't update.
* Bug fix: Charts don't align the zero axis line for both primary and secondary axes.
* Bug fix: Grid chart : Sorting is not working,if we sort on attribute of numeric datatype.
* Bug fix: Micro Chart:Tooltip shows wrong values when compared to actual data.
* Bug fix: Font set on property editor doesn’t override font from customStyles.css in specific charts for axis labels.
* Bug fix: Charts with default gradient threshold: Legend shows wrong values with percentage metric.
* Bug fix: Color picker shows default color as blue even if series color is different.
* Bug fix: MSTR Update-4: In web library edit mode, increment/decrement arrows are not showing up.
* Bug Fix: MSTR 2021 Update-4: In web library edit mode, marker window is not showing any markers icons.

### **5.0.3**



* Bug fix: Security fixes related to possibility of cross-site scripting attacks (XSS) in different places of the VitaraCharts editor where user input was required.

### **5.0.2**



* Improvement: The feature to adjust the spacing between the bars/columns is upgraded.
* Improvement: Formatting capabilities for legend where you can wrap text.
* Improvement: On the chart properties window, the scroll bar is now positioned at the top while switching to another tab in the property menu.
* Bug fix: The number format in the web library is different from the web for German (Switzerland) users.
* Bug fix: In the bubble and Waffle charts custom SVG markers are not working.
* Bug fix: Bubble chart: Bubble size is not considered if the series is edited before adding metric to bubble size.
* Bug fix: Bubble chart: Pattern fills are not working in the bubble chart with bubble size metric.
* Bug fix: Bubble chart: Pattern fill is not working for some markers (fontello) in the bubble chart.
* Bug fix: Pie chart: The chart disappears showing white space, when we enable attribute form and enable gradient option in the series.
* Bug fix: Pie chart: When we click on a slice, the legend is highlighting the wrong element.
* Bug fix: Pie chart: When we click on any slice the entire legend is disabled.
* Bug fix: Gradient fill + Smooth line: Enabling or disabling the smooth line causes colors in the gradient fill to reset to default blues.
* Bug fix: Polar mode doesn't retain Gradient color when chart type is changed from Bar to Column.
* Bug fix: Data labels not displayed on horizontal bars and pins in trendline in grid chart and micro chart.

### **5.0.1**



* Bug fix: Upgraded to use a newer version of a third party library (Apache commons) that fixes a potential security vulnerability.

### **5.0.0** <a href="#user-content-5.0" id="user-content-5.0"></a>



* New Feature: Gradient color fill can be added where the series property is available.
* Enhancement: Bar Chart has now an ability to display fill percentage.
* Enhancement:For bar and column charts, the series property now includes a Delta bar feature.
* Enhancement: Added an unfilled Color option to the Waffle Chart.
* Enhancement: Ability to use Sankey charts vertically.
* Enhancement: In bubble chart you can now use a separate marker for each series.
* Bug fix: When the series property is modified, the bubble chart legends likewise change color.
* Bug fix :Fixed the marker size, which used to look small in comparison to other bigger values.
* Bug fix : Disabled DeltaBar in case of Polarmode, Dynamic width, Overlay, IBCS view & Play-Axis.
* Bug fix :Bar Fill is not working for Negative Metric.

### **4.9.3**



* New Feature: Vitara Charts icons now can be seen in relevant tabs (Menus) while choosing new visualization (only works with MicroStrategy V11.3.05 and above).
* Enhancement: Thresholds feature in waffle chart.
* Enhancement: Bubble chart: Added Option to turn on transition lines between trail Sequence and current Sequence. The option to enable this feature is available in the Play-Axis tab.
* Enhancement: Changed name "Show Sequence" to "Retain Points" in Play-axis Tab in all charts.
* Bug fix: Recreated build using updated build scripts to remove unwanted files added since 4.9.2.
* Bug fix: Dumbbell Chart: Thresholds appear black on the target section.
* Bug fix: Data marker: In the series tab when we set data markers as series, the size of the markers is changing according to the metric value. Now the markers to be of constant size.
* Bug fix: Vitara charts not showing correct percentage values on axis labels.
* Bug fix: Vitara Grid chart in iPad: When data has attribute groups, then in the iPad library and mobile apps grid chart is not rendering and showing an error message.
* Bug fix: The tooltip is going behind the toolbar in MSTR web.
* Bug fix: Pie chart: The datalables becomes clumsy if we select the play axis show sequence option "First/Last but one".
* Bug fix: Slope chart: If we enable show axis on right and then disable this option we are getting value axis in metric formatting.
* Bug fix: Backward compatibility: previously chosen sequence now show selected in property editor Play-Axis tab.

### **4.9.2**



* New Feature: Horizontal and verticel totals feature is added to the Heatmap chart and it’s formatting option ia available in the Data label tab in property editor.
* Enhancement: Stacked bar/column charts and mekko chart: In the data labels menu 'Stack total/header label' option is renamed to 'Total Labels'.
* Enhancement: Stacked bar/column charts, heatmap and mekko chart: Now we can enable/disable 'Total Labels' independently from the option ‘All’ in the data labels menu.
* Bug fix: Tooltip is covering the enire chart.
* Bug fix: Vitara charts are not hiding null values.
* Bug fix: Data labels rotation is not working in the waterfall chart.
* Bug fix: Waterfall Chart: 'Add Link' feature is getting applied but not allowing to click on it.
* Bug fix: Pattern fill feature is not working in the thresholds.
* Bug fix: Threshold color is not being applied if pattern fill is selected for series.
* Bug fix: Bar Chart: When small multiples feature is enabled and variance property applied the data labels appear double times (clumsy).
* Bug fix: Series and threshold tab show only last unit series when small multiples is enabled.
* Bug fix: Enabling small multiples on variwide chart breaks the chart.
* Bug fix: Slope chart doesn't render when small multiples is enabled with category axis on both sides/right side.

### **4.9.1**



* Bug fix: Export Vitara charts to pdf is not working in MicroStrategy version 2021 5.1 (11.3.05).

### **4.9.0** <a href="#user-content-4.9" id="user-content-4.9"></a>



#### New Features/Enhancements:



* New Feature: Pattern fill option (Grid/Square/Double Square) in the series tab.
* Enhancement: Rotation Option for data labels.
* Enhancement: Play axis UI modified. Moved “show first sequence & penultimate sequence” options to property editor under play-axis tab 'Show Sequence' selection option.
* Enhancement: Added “Play Axis” tab in Property Editor for play-axis supported charts (column chart, pie chart, line chart, area chart, bubble chart, tornado chart, sparkline chart, funnel chart, column range chart, and bullet chart).
* Enhancement: Custom data markers support in the data labels applied from thresholds.

#### Bug fixes:



* Bug fix: Column chart: If we enable drill target, tooltip is showing like "Undefined".
* Bug fix: Column chart : If we Varience, then the already applied series 'line' is not showing properly in the properties tab.
* Bug fix: Grid chart: The position/order of metric column is changing when we rename a metric.
* Bug fix: Grid chart: In grouped mode, the chart is sorted in reverse order if sorting is cleared after it is applied once.
* Bug fix: Custom SVG marker used in the series tab, are not appearing at the correct position in the Export to pdf file.
* Bug fix: Dumbbell chart: The Connecting lines between two points doesn’t appear while small multiples enabled.
* Bug fix: Tornado Chart: Data Labels shows opposite values when selected minimum and maximum values to display on the chart.
* Bug fix: iPad mobile and library apps: If series is drawn using the attribute, then changes done in the series tab are not working in iPad/android.
* Bug fix: Document in mobile apps : For waterfall chart the "down value color" is showing as " Up value color".

### **4.8.6**



* Bug fix: Custom font issues with label positioning in web, rendering differences in library and export scenarios.
* Bug fix: Small multiples backward compatibility fix: Disabled share category axis in small multiples for charts saved before 4.8.3. (IBCS charts will have share category axis option enabled).
* Bug fix: Web Library (MSTR 2021 U-4.1): Grid Chart column data is not aligned with column headers.
* Bug fix: Web Library (MSTR 2021 U-4.1): Grid chart - column background color is overlapping with the beside column.

### **4.8.5**



* Bug fix: MicroStrategy 2021 update-4.1: In dossiers Vitara charts are not rendering in the IPad library app.
* Bug fix: Vitara waterfall chart is showing the value 2.37% as 2.36%.
* Bug fix: Stacked bar/column chart: Tooltip is showing value for one of the metric values only.
* Bug fix: Stacked bar/column chart: Tooltip showing some big random numbers in short format.
* Bug fix: Stacked bar/column chart: When the metric format is set to 'Use metric format', the tooltip is showing the first element value, instead of aggregated sum.
* Bug fix: Line/area chart: Line style for smooth line in line and area charts is not working.
* Bug fix: Vitara charts showing error message when Month of year attribute is placed in the small multiples.
* Bug fix: Bar chart: In the exported PDF file, the plotline created at the 0 axis value is shifting onto the bars when we have custom fonts applied the chart.
* Bug fix: Vitara grid chart: Problem in displaying the formatting of the aggregate value (after copying from the 'chosen column') is not correctly retained in the case of time metric.
* Bug fix: Web documents: IBCS view in small multples mode with null values chart is showing an error message.
* Bug fix: IBCS view: Problem in category axis labels alignment when there are nulls for some of the categories of the first small multiples element.

### **4.8.4**



* Bug fix: Fixed rendering issues in the edit mode of the web libarary in MicroStrategy2021 update-4.

### **4.8.3**



* Bug fix: In all the charts an invalid state error occurs while one of the following actions is made in quick succession (driving chart using attribute/metric selectors, add/remove dropzone items, switching between charts, or any set of property changes that could trigger multiple chart redraws).
* Bug fix: Column chart: If radius has given some value, the polar mode appears differently in export to pdf.
* Bug fix: Color picker input supports RGBA and ARGB color codes for optional transparency.
* Bug fix: Grid chart: 'Precision' setting is not working with 'Ratio' value aggregation.
* Bug fix: Grid chart: Apply a threshold using a metric. Later rename the metric. The applied threshold will disappear from the chart.
* Bug fix: Bar chart: Category axis labels cutting off in the exported pdf.
* Bug fix: Bubble chart: If attributes are input to the horizontal and vertical axis drop zones then the vertical axis is showing some random.
* Bug fix: Custom SVG markers are not appearing in the correct place when used in series.
* Bug fix: Custom SVG markers are not retaining their original positions after zoom-in and zoom-out.
* Bug fix: IBCS mode with small multiples enabled: Inconsistent category axis across charts when the data in each chart is different or have nulls.
* Bug fix: Stacked bar/column:After converting to area chart, in the series tab, edit a series and change its color. The applied color will not display on the chart.

### **4.8.2**



* Bug fix: Area/Combination chart with area chart: Custom color is not being applied to transparent area.
* Bug fix: IBCS small multiples error - _unequal data lengths found_
* Bug fix: Grid chart: Chart is showing error message when thresholds applied i a particular scenario.
* Bug fix: Enabling smooth line for one series affecting others.
* Bug fix: Stacked Area chart Backward compatibility: Coloring opacity is not retained correctly in 4.8.

### **4.8.1**



* Bug fix: Tornado chart: Value axis is showing more space in the left side than right side.

### **4.8.0** <a href="#user-content-4.8" id="user-content-4.8"></a>



#### New Features/Enhancements:



* New Feature: Introduced Smooth line option for line/area/sparkline charts.
* New Feature: Introduced smooth line option in the series tab of the line, area, bar, column and Stacked bar/column chart.
* Enhancement: Added support for attribute macros in the angular gauge chart.
* Enhancement: Added Plotlines menu to waterfall chart, plotlines can be added on metric sources in waterfall chart.
* Enhancement: Axis label rotation can be applied independently on parent and child attribute levels.
* Enhancement: Added a default rotation option for labels in the property editor.
* Enhancement: If multiple date categories are present and the rotation of level 0 label set to 0, show only the first date of the parent category (year/ month).
* Enhancement: Transparency to area chart based on overlapping. Series will be transparent if it overlaps with others, else opaque.
* Enhancement: Waterfall chart: Ability to display value axis line at 0 value. Currently, there is no option to add 0 line.

#### Bug fixes:



* Bug fix: Grid chart: Attribute column shrinks its size when we do 'Move to Column' on second attribute.
* Bug fix: Grid chart: Applying thresholds with cell background color, is not coloring the entire cell background. Leaving some part of the cell with default white color.
* Bug fix: Sankey chart: Dissimilarity between web and mobile when Use as filter is applied on the target node of the sankey chart.
* Bug fix: Bubble chart: Issue with the feature to add attributes to the horizontal and vertical axes.
* Bug fix: If the dossier is 'Save as' a new file then changes applied in the series tab are not restored in the newly saved dossier.
* Bug fix: Waterfall: Second metric is splitting into the attribute in the 'Group by' dropzone, even if there is no attribute in the 'Break by' dropzone.
* Bug fix: Waterfall chart: Category axis labels and Data labels are not fully visible after enabling small multiples.
* Bug fix: Waterfall chart: In the horizontal axis mode, axis labels are truncated when axis label rotation is reset to '0'.
* Bug fix: Waterfall chart: Category axis labels are not fully visible after enabling small multiples.
* Bug fix: Data labels of positive values are showing left side of the zero axis.
* Bug fix: Stacked bar/column charts not showing percentage values in the secondary axis.
* Bug fix: In all charts, the delete option in the series tab is not working.

### **4.7.8**



* Bug fix: Sankey chart filtering issue in library mobile.
* Bug fix: After 'Save as', tooltip is showing Object ID of the derived metric.
* Bug fix: With the new error handling mechanism, which is implemented in 4.7.6, all the warning messages got replaced with a common error message.

### **4.7.7**



* Improvement: Grid Chart: Disabled metric labels in pivot header, while chart rendered using single metric.
* Bug fix: Grid chart: Header style options in the appearance tab are not applied to pivoted headers.

### **4.7.6**



* Enhancement: Implemented better error handling feature.
* Bug fix: Grid chart: Horizontal bars/pins are not scaling equally for positive and negative data.
* Bug fix: Grid chart: If set end value for trendlines, the tooltip (group tooltip )is showing wrong values.
* Bug fix: Grid Chart: Custom svg markers are not fully visible. Bottom part of the markers is hidden/clipped.
* Bug fix: Grid chart: Columns turn blank after applying custom markers, if vertical font alignment is set to 'bottom' or 'middle'.
* Bug fix: Grid/Micro Custom Markers: Fill menu in custom markers tab is not opening.
* Bug fix: Grid/Micro: Trendline is not taking full width of the cell.
* Bug fix: Micro chart: Horizontal bars and Horizontal pins are not working.
* Bug fix: Locale related: Already applied attribute thresholds are not editable in german locale.
* Bug fix: Locale related: Plot line editor is not showing the source metric name when opened in the german locale.
* Bug fix: Locale related: In non-english locales, legend is showing incorrect names.
* Bug fix: Compatibility issues/errors between enable playAxis, variwide, variance views. Either of these three options can’t be enabled at a time, property editor fields will update accordingly.
* BugFix: In all high charts, a small box is displaying on the chart when we hover for the first time on the chart.
* BugFix: Bubble Chart: Plotline title alignment is not working correctly for vertical plotlines.
* Bug fix: In the SSO enabled server, background images are not working in mobile devices.
* Bug fix: In the series tab, if we apply data markers as series, markers (in-built marker) are not showing up in the ipad library and mobile applications.
* Bug fix: ‘About’ option is removed from the context menu.
* Bug fix: Chart properties applied on derived metrics are not retained after “Save As” new document.
* Bug Fix: Charts are showing error when only subtotals are added to the chart or an attribute has only one element ‘Total’ in the data.
* Bug fix: Sankey chart freezes on hovering over links with large datasets.
* Bug fix: backwards compatibility issue with thresholds and plotlines for versions since 4.7.1.
* Bug fix: Edit button is not visible when MicroStrategy totals/sub-totals are enabled.
* Bug fix: Charts show an error on ipad when one of the attribute element is named ‘Total’.

### **4.7.5**



* Bug fix: Stacked chart: Threshold functionality is not working on the series created using the second metric.
* Bug fix: Stacked Column chart with metric series: In Threshold editor is distrubbed.
* Bug fix: Attribute plotline: The macro &\[plotline.value] is not working correctly.
* Bug fix: Custom background color for tooltip is not applied consistently.
* Bug fix: IBCS point placement format is changing with change of container size.
* Bug fix: In all charts, select target feature is not working correctly when element data is replaced using Microstrategy's advanced threshold editor.
* Bug fix: When we add metrics to rows or attributes to columns, VitaraCharts used to show error message. But from 4.6 this is not working.
* Bug fix: Sankey, Missing nodes when node column has tens of data points. Fixed by auto adjusting node padding and curve factor of links.
* Bug fix: Waffle Chart: Click on custom svg markers does not highlight the selection.
* Bug fix: Already applied Custom Markers are breaking or changing into unknown markers when we edit anything in the series Editor.
* Bug fix: Force sort axis data option is not working correctly if we have numerical values in the category axis.
* Bug Fix: Android Specific Bug: In web documents, charts are not showing secondary axis, marker, and thresholds in android.
* Bug fix: Time format hh:mm:ss on value axis of the line chart is not working.
* Bug fix: In the small multiples mode, legend does not work as a Selector.
* Bug fix: Vitara Text box goes blank when we use multiple attributes with multiple attribute forms.
* Bug fix: Grid chart: Pivot + Variance chart --> '0' values are displayed in red color.
* Bug fix: Grid Chart: New trendline charts getting color of the earlier applied chart.
* Bug fix: Grid Chart: Bars thresholds is using target data for bars.
* Bug fix: Grid Chart: Bar width of the threshold is incorrect with marker only option.
* Bug fix: Grid chart: The chart breaks when custom markers are applied on Grouped rows.
* Bug fix: Bullet: The error "TypeError: this.setYAxisDurationFormat is not a function" occurs on the chart by default.
* Bug fix: Unauthorized access issues with config.aspx
* Bug fix: In mobile, metric series is not showing in stacked charts.
* Bug fix: Custom properties from global.txt are not working in mobile.
* Bug fix: Unable to edit series options for Sankey chart.
* Bug fix: Unable to edit series options for Pie chart.
* Bug fix: Waffle backward compatibility: Error occurs on the chart when applied custom svg marker does not exist in the server.
* Bug fix: Custom svg marker view (prop menu) does not translate text into the locale specific language.
* Bug fix: Removed support for Absolute urls (external links) in custom svg markers while Exporting and in Desktop, fixes export internal errors issue.
* Bug fix: Updated missing string translations which are removed in 4.7 (these are present in 4.6.4).
* Improvement: Waffle chart: Improved performance of rendering in grid mode with custom svg marker selected.
* Imptovement: Grid chart: Change the names of the options for variance and % variance to horizontal bars and horizontal pins respectively.
* Improvement: Added support for using absolute urls (svgs from web) in custom svg markers.

### **4.7.4**



* Bug fix: In MSTR 2021 Update-1, Vitara grid chart with dark theme and blue theme does not correctly display the grid headers.
* Bug fix: Grid chart: Grand Totals are missing from the PDF exports

### **4.7.3**



* Bug fix: Unable to open Edit property window on MSTR-2021 Update-11.3.1 with SSO authentication.
* Bug fix: Grid chart: Error on clicking on column menu > Filter Data option.

### **4.7.2**



* Bug fix: Markers not loading in mobile library when web server is on IIS and library server is on tomcat.
* Bug fix: Server url without “/” at the end is not accepted for mobile and library configuration.
* Bug fix: Updated use of configured URL to be consistent in library export.

### **4.7.1**



* Bug fix: Waterfall chart: TypeError: cannot read property ‘getTValue’ of undefined.
* Bug fix: Waterfall chart not rendering correctly with null data metrics.
* Bug fix: Data indicator options in waterfall not applied.
* Bug fix: Grid chart: Background color of the grouping headers reverts back to the original.
* Bug fix: Grid chart: Apply background color for headers then create a column group. The top headers row will not be in the applied headers background color.
* Bug fix: Grid chart: HTML image tags as attribute forms are not supported in Vitara Grid.
* Bug fix: Micro Chart Backward Compatibility: Line chart trendline scale changes after upgrading to 4.7 from 4.4.6.
* Bug fix: In web documents, most of the charts are giving an error when each attribute form is formed as a separate column.
* Bug fix: Sorting issues with Multi-tier Bar chart.
* Bug fix: Dual axis line not rendered with relative variance view.
* Bug fix: Outlier formatting is not applied to relative variance view.
* Bug fix: Bar/column charts looks different in web and mobile when variance is enabled.

### **4.7.0** <a href="#user-content-4.7" id="user-content-4.7"></a>



#### New Features/Enhancements:



* New Feature: Added support for stack by area charts in stacked chart. New property "chart type" is introduced under series tab in stacked bar/column.
* New Feature: Integrated absolute variance and relative variance views into bar and column charts.
* New Feature: Grid/Micro Chart: For the trendlines, option to set axis minimum and maximum values for the scaling.
* New Feature: Grid chart: On trendlines, now we can set a group of metrics having the same vertical axis scaling. To enable this fetaure, go to the hamburger menu -> Grouping -> Manage Scaling Grouping.
* New Feature: Grid Chart: Introduced variance chart and variance Percentage Chart.
* Enhancement: Grid chart: New option 'Clear scaling grouping' in the reset columns property, in the reset columns context menu, and in the hamburger menu.
* Enhancement: Grid/Micro chart: How to standardize that the Y axis of all the metrics will scale according to the same axis values in the micro chart.
* Enhancement: Grid/Micro: For the display as bars/lines/bullet, enable a way to sync the scales across columns.
* Enhancement: Added a new option in the data labels menu to force outlier labels outside when “show labels outside” is set to true.
* Enhancement: Ability to use attributes in horizontal/Vertical axes in the bubble chart.
* Enhancement: Improved series options handling by using column/element Ids, fixes issues with locale change in color by scenarios.

#### Bug fixes:



* BugFix: D3 library of vitara charts overwriting an existing d3 object on the window.
* Bug Fix: Grid chart: When only metrics in the chart, grid chart is not showing any rows.
* Bug Fix: Grid chart backwrd compatibility: Create a grid chart in 3.9 version with one attribute grouped and then open it in 4.3, 4.4, and 4.5 versions then the grouping is lost.
* Bug Fix: Grid Chart and Micro Chart: Chart breaks with irrelevant error message if two attributes or metrics have the same exact name + Column order.
* Bug Fix: Grid Chart: Threshold condition showing values based on target instead of source.
* Bug Fix: Grid/Micro Chart: Customer don't want to show the detail row when all the attributes in the chart are grouped.
* Bug Fix: Grid chart: The group aggregation value 'clear' option is not working when we apply pivoting on attributes or metrics.
* Bug Fix: Gird chart in mobile: Unable to expand column grouping.
* Bug Fix: Grid chart: iPad library app is showing empty chart when attribute thresholds are applied with Custom SVG markers.
* Bug Fix: Grid Chart: When grid chart is exported to pdf then all the column groups should be expanded state.
* Bug Fix: Grid and Micro Chart: Tooltip editor changes are not affecting the tooltip which shows on group aggregations.
* Bug Fix: Grid Chart backwrd compatibility: Chart state not restoring from 3.9 and before.
* Bug Fix: Grid Chart: Drag and Drop zones for Grouping and Pivoting are not getting translated into locale specific language.
* Bug Fix: Grid Chart: Context menu theme names are not getting translated into locale specific language.
* Bug Fix: Grid Chart: Some options in Hamburger menu are not getting translated into locale specific language.
* Bug Fix: Grid & Micro charts: trendlines height is getting affected if we set vertical font alignment.
* Bug Fix: Fixed filter issue with sankey new data model format (when source and target attributes selected from Sankey Menu).
* Bug fix: In the global.txt file, if we use double quotation for the custom font names(font names with multiple spaces), only the first custom font is showing in the property editor.
* Bug Fix: Bar Width for Polar Mode is not working (no specific fix was made, should have been fixed while refactoring other issues).
* Bug Fix: Drill chart: Error opening target property editor when chart type is set to pie.
* Bug Fix: In mobile (Library & Mobile Apps) the macro &\[Category@DESC] is not working.
* Bug Fix: KPI Ring chart: Legend color is not the same as the chart color.
* Bug Fix: Use as Filter is not working in the IPAD Library app if multiple attribute forms are enabled in the attribute.
* Bug Fix: Vitara charts Inconsistency between web and mobile when multiple attribute forms are enabled.
* Bug Fix: Removed the bubble size zone requirement with at least one metric in the chart.
* Bug Fix: Adding only metrics to tooltip dropzone.
* Bug Fix: Simple KPI: small multiple : Threshold property "check across all charts" is not showing correct value.
* Bug Fix: Simple kpi small multiples: thresholds created in previous versions are not applied on the chart.
* Bug Fix: When there is only one data point in the secondary axis, the secondary axis label is not showing in the short format.
* Bug Fix: Simple KPI backward compatibility: Small multiples title formattings are not retained in web documents.

### **4.6.6**



* Bug fix: Vitara GridChart shows no data when there is no attribute used (and only metrics are added to the grid).

### **4.6.5**



* Bug fix: Error on enabling waterfall delta view in waterfall ibcs mode.
* Bug fix: Fixed issues with broken axis view for aggregate series elements in IBCS Multi-tier column chart.
* Bug fix: Fixed issues with aggregate data labels and series not rendering in IBCS Multi-tier bar chart.
* Bug fix: Fixed issues with primary and secondary series grouping to IBCS standards.
* Bug fix: Inverted markers in IBCS Multi-tier column scatter.
* Bug fix: Removed restrictions to overflow data labels to be justified inside the graphic.
* Enhancement: Added contrast color to justified data labels.

### **4.6.4**



* Enhancement: Column range chart: Added support for using custom date format in the axis labels. Added new options to set the desired date format in the column range tab.
* Enhancement: Updated language translation for all property menu text.
* Bug fix: Vitara Charts are not working on MAC OS 11.
* Bug fix: URL API links in attributes are not working when the link is not hardcoded to the target environment.
* Bug fix: In german locale, calendar heatmap is not working with date format DD.MM.YYYY.
* Bug fix: Histogram Backward compatibility: Positioning of the cumulative sum line and markers changed in 4.6 compared to previous releases.
* Bug fix: Plotlines using attribute in conbination with thresholds are not applying when threshold target is metric, source is attribute with plotline using any condition.
* Bug fix: Stacked charts backward compatibility: With 'stack by percentage', the stack totals are not displaying outside the bar/column.
* Bug fix: Waterfall chart: Fixed locale related issues.
* Bug fix: Waterfall chart: The data labels are not displaying outside the bar if 'deduct value' is enabled for a group.
* Bug fix: Waterfall chart: Save As new dossier not retaining state of metric groups and group options.
* Bug fix: Grid chart: Attribute thresholds are not working when metrics pivoted to rows.
* Bug fix: Grid chart: Thresholds on metrics not working after metrics pivoted to rows.
* Bug fix: Grid chart: Thresholds on bars are not plotting correctly when we have null values and zero values in the metrics.
* Bug fix: Grid chart: Custom SVG markers in thresholds are not working when we have threshold target as a negative values metric.
* Bug fix: Grid chart: Null values + Custom markers(display style), the chart breaks.
* Bug fix: Grid chart: Attribute thresholds are not applying correctly when there are special characters.

### **4.6.3**



* Bug fix: Performance issues (specific to Internet Explorer) while loading dossiers in library

### **4.6.2**



* Bug fix: Grid Chart: 'Equal to' operator is not working for thresholds on metrics in Grid
* Bug fix: Bar/Column charts: Long category labels are not wrapped or truncated and cause the charts to take up a lot of space

### **4.6.1**



* New Feature: Grid Chart: From 4.6.1 release usres can apply custom SVG markers in the thresholds.
* Enhancement: Grid Chart: Until 4.6.0, the source and target of the thresholds were always metrics. Now the source of the thresholds can be an attribute.
* Enhancement: Small Multiples: Option to enable/disable chart title.
* Enhancement: Simple KPI: Chart title style is merged with small multiple title style even when Small multiples is not enabled.
* Bug Fix: Attribute thresholds and plotlines are not working with special characters in the values.
* Bug Fix: Added support for MSTR date formats in the german locale.
* Bug Fix: Fixed CSRF security vulnerabilities.
* Bug Fix: German locale: Column range chart: Custom date formats are not working.
* Bug Fix: Sankey backward compatibility: The issue with data labels as 'show overlapping labels' option is not working.
* Bug Fix: KPI Ring Chart: Exported pdf file is showing an error message if we enable legend in the chart.
* Bug Fix: Start Angle and End Angle options not working when small multiples are enabled.
* Bug Fix: Formatting issue with stack Totals in the stacked bar chart.
* Bug Fix: Grid Chart: Threshold range option not disappearing.
* Bug Fix: Grid chart: 'Equal to' condition in Attribute thresholds is not working for the 'Numeric value attributes'.
* Bug Fix: Line chart: Marker direction is changing after setting 'Bar' as series
* Bug Fix: Simple KPI chart: Small multiples title font properties are changing with the data labels menu title options.
* Bug Fix: Marker property in context menu does not work on the specified series.
* Bug Fix: Simple KPI: Charts are not showing title in small multiple configurations.
* Bug Fix: Micro Backward Compatibility: The trendline scaling changed in 4.6 for the charts created in 4.3.4
* Bug Fix: Grid Chart: Column names with \<or > characters, are unable to format in the column formatting menu.
* Bug Fix: Micro Chart: Move a metric to left and refresh the chart, chart groups by metric.
* Bug Fix: Variwide chart: If the metric name contains < or > characters, then they are escaped in the property editor where the option to enable variwide is present.
* Bug Fix: All charts: Axis labels are extending into the chart area.
* Bug Fix: Horizontal Waterfall: By default, category axis labels are overlapping.
* Bug Fix: Waffle chart: The < and > characters are showing as > and < in the header labels (List and grid modes).
* Bug Fix: In small multiples, Primary value axis shows title of secondary value axis.
* Bug Fix: Line chart: Marker direction is changing after setting 'Bar' as series.
* Bug Fix: Stacked bar/column: enable marker option(used with line/area series) is not hidden for datamarkers series type.
* Bug Fix: Bar chart: With line series, the marker is changing when hovered onto a data-point.
* Bug Fix: Backward Compatibility Issue: For charts with markers enabled in thresholds, when we edit the threshold, the marker selected is not restored.
* Bug Fix: Pie chart: In series property, the attribute element name is missing.
* Bug Fix: Colors applied with opacity other than 100% are restoring as black irrespective of selected color in the property menu.
* Bug Fix: Marker type under series properties is always set to circle, irrespective of the selected marker.
* Bug Fix: In the appearance property, the opacity option of chart area and plot area color is not working.
* Bug Fix: Bullet chart: when we double click on an attribute, the attribute will be placed into the Category axis drop zone. But in the bullet chart this is not happening.
* Bug Fix: Line Chart Backward Compatibility Issue: For charts created in 4.0.5, the gradient threshold marker is changing to default in 4.5.2.698

### **4.6.0** <a href="#user-content-4.6" id="user-content-4.6"></a>



#### New Features/Enhancements:



* New Feature: Attribute Thresholds, attribute elements will now be available as source elements while creating thresholds and also supports attribute dates with date selectors.
* New Feature: Attribute plotlines/reference lines: Attributes can be used to draw plotlines in the chart.
* New Feature: Variwide chart mode is implemented in the bar and column charts.
* New Feature: Polar mode options added to column, bar, line, sparkline, area, stacked bar and stacked column charts.
* Enhancement: Funnel chart: Ability to show the data labels inside the funnel.
* Enhancement: X-Axis grid line property, now gridlines can be added to x-axis as well.
* Enhancement: Grid chart: The threshold editor tab is modified with the name of the label for selecting threshold source.
* Enhancement: Enabled “Context Menu” in global.txt by default.
* Enhancement: Grid chart: Rows that have only one element(all attributes applied grouping), will not show the arrow.
* Enhancement: Bar/Column/Stacked Bar/Stacked Column/Line/Area/Sparkline charts will have a new tab in the properties pop-up window. The options related to bar widths/line width etc., are moved to this tab from the appearance tab.

#### Bug Fixes:



* Bug Fix: Bullet chart: Improved bullet drop zone transition when a visualization is converted to a bullet chart.
* Bug Fix: Bullet chart: Bands are not working correctly with negative values.
* Bug Fix: Sorting related issues in the sanky chart
* Bug Fix: Grid Chart: Custom markers don't honor the font size.
* Bug Fix: In the MSTR-2019 server grid chart is showing the right click menu options even when the global.txt file dont have the flag.
* Bug Fix: Legend styles not applied when small multiples mode is enabled.
* Bug Fix: Simple KPI chart: The fixed font sizes are not adjusting as per the screen resolution.
* Bug Fix: Stacked charts showing non-existent values on the category axis.
* Bug Fix: global.txt file updated in library and mobile builds.
* Bug Fix: Earlier we used to have an option to enable markers for series, this is no longer available in 4.5.6.
* Bug Fix: Setting for secondary axis under Series tab are not retaining when the dossier is copied or saved as to another version.

### **4.5.6**



* Bug Fix: Sankey chart - Chart shows error on applying series options or thresholds using the attribute name or attribute elements with special characters.
* Bug Fix: Vitara charts are not showing the 'Edit' button when “accessControlLevels” enabled in the global.txt file and if the document/dossier name contains xml characters like (&, <, >, etc).
* Enhancement: Grid chart: Support for custom SVG markers in the display as tab.
* Bug Fix: Micro Chart: Tooltip display is outside the Dashboard.
* Enhancement: Added guidlines using custom markers in the Background and Custom SVG tabs.
* Bug Fix: SVG data markers are not rendering in the ipad library and mobile apps.
* Bug Fix: The size of the data marker is not showing correctly in web library.
* Enhancement: Updated vitara.co domain references to vitaracharts.com
* Bug Fix: Removed note in dataMarker Options.
* Bug Fix: Data markers options - fill, disabling aspect ratio and repeat marker are not working in all mobile environments.
* Bug Fix: Calendar heatmap: In IE when we hover the cursor between the months, the chart is blinking.
* Bug Fix: Android Library App: Tooltip is not showing in D3 charts.
* Bug Fix: If data is in the date format DD-MMM, Vitara chart is drawing one bar for multiple dates.
* Bug Fix: Drill chart: Charts does not render and show a console error when the target chart is maximized/ minimized.
* Bug Fix: Vitara Waterfall showing Object Object for blank Metric Name.
* Bug Fix: Waterfall Backward compatibility: Chart created in 4.5.0, Category axis is sorted in reverse order in 4.5.4.712.

### **4.5.5**



* Bug Fix: SimpleKPI: Horizontal alignment of labels not working in Firefox.
* Bug Fix: MSTR 2019: Vitara Charts in different panels are not updating with the selection made in the selector.
* Bug Fix: KPI Animation backward compatibility: The chart created in 4.0.5, the text formatting options bold and italic are auto applying in 4.5.4 version.

### **4.5.4**



* Bug Fix: Tooltip is not showing for the attribute names in French.
* Bug Fix: Tooltip not working correctly when D3 chart has metric with NULL values.
* Bug Fix: In the Android Library app, the tooltip is not showing for all D3 charts.
* Bug Fix: Custom markers in the exported to PDF file are appearing smaller in size than in the dossiers.
* Bug Fix: Using svg files as data markers is not working.
* Bug Fix: Data markers are showing in the reverse direction.
* Bug Fix: KPI Animation: In text formatting properties, the Font, Font size and Italic, Underline options are not working.
* Bug Fix: Stacked bar/column chart: Add attribute to color by. Add new series to a metric. Remove the applied color by. Metric series is retaining and the data that has to be stacked is also merged with metric series.
* Bug Fix: The export of Vitara Line Chart to PDF from Dossier doesn’t export all data.
* Bug Fix: Micro chart: Manually adjusted column width is not saving the state.
* Bug Fix: Micro Chart: Resize the row-group column by dragging the column, now refresh the chart. The column goes back to the previous width.
* New Feature: Grid Chart: For the line and bar display styles, users can select the specificity of the axis. Two new options added in this context: a) Same across cells and b) Apply at each cell.
* Bug Fix: Grid Chart: MSTR 2020 context menu not working properly for fit to content.
* Bug Fix: Grid Chart: From the MSTR 2020 context menu, if we apply ‘fit this to content’, it is not saving state.
* Bug Fix: Grid Chart: Move metrics to rows and group by Metrics collection. Apply custom markers on any of the metrics. The markers will fail with an error message.
* Bug Fix: Grid Chart: The detailed rows are not showing any values in the following scenario. Clear aggregation of a metric and show trendline charts.
* Bug Fix: Grid Chart: Row group expansion is not saving state.
* Bug Fix: Waterfall: The options in the waterfall menu are not working in mobile environments.
* Improvement: Waterfall: Improved tooltip position issues with waterfall when there is a start or end value set to the value axis.
* Bug Fix: Waterfall: Data labels position for negative values / deduct values is shown on the higher side of the bar except in the IBCS mode.

### **4.5.3**



* Bug Fix: Waterfall Auto compute start value not working with nonadditivies.

### **4.5.2**



* Bug Fix : Waterfall chart: In the vitara 3.7 version, if we apply the start value on the value axis, and open this chart in later versions, the chart will not show the start value as we customized.
* BugFix : Grid chart: Use as filter is not working properly when the "Show Totals" option in the MSTR grid is enabled.
* BugFix: waterfall null metric data label showing 0 when custom formatting is applied
* Bug Fix: Android Documents: For line chart, secondary axis is not showing in android library and mobile app
* Bug Fix: Attribute Name not visible in French on Tooltip
* Bug Fix: No Data Returned taking up the entire viewport for some charts
* Bug Fix: Vitara charts of version 4.4 are not showing right-click menus in presentation mode.
* Bug Fix: Text Node : attribute form macros not working in Text Node chart.
* Bug Fix: Grid Chart: Backwards Compatibility for clear aggregation + pivot column
* Bug Fix: Grid Chart: Row group column is not restoring column order state
* Bug Fix: Grid Chart: Column grouping with Total column broken
* Bug Fix: Grid Chart: Reset column in property editor breaks with error message
* Bug Fix: Grid Chart: Grouped column loses pinned state
* Bug Fix: Grid Chart: Trendline tooltips show wrong value in Metrics to rows state.
* Bug Fix: Grid Chart: Metrics collection is losing grouping state.
* Bug Fix: Micro Chart: Grouped column not retaining styles after refresh
* Bug Fix: Micro chart: When we refresh two times the micro chart, the pin column for the grouped column is not retaining its state.
* Bug Fix: Micro chart: Unable to resize the row grouped column in the micro chart.
* Bug Fix: Micro chart: In trend lines bar chart options, the negative color is showing as Ash color and the applied color is Red color.
* Bug Fix: Column Backward Compatibility: Markers for thresholds are not showing on line series in 4.5 for charts created in 4.0.
* Bug Fix: Bullet chart: If we draw vertical bars, the category axis is showing the elements inversely
* Bug Fix: Heatmap: default color is not applied.
* Bug Fix: Heatmap is showing colored cells for null values also.
* Bug Fix: Bars are overlapped with each other when updated to 4.4.1
* Bug Fix: Value axis labels: Negative value axis labels are not showing $ sign
* Bug Fix: Column Range: The chart is not displaying bars if start metric value is zero.
* Bug Fix: Line chart Backward Compatibility: Marker is not displaying for zero values.
* Bug Fix: Play axis: If we apply loop then we are unable to see last element graph.
* Bug Fix (partial - specific to customer reported): The > character is showing as \&gt;
* Bug Fix: After applying data markers if we apply thresholds using markers, threshold markers are not showing in the chart
* Bug Fix: Angular gauge chart: By default, with the percentage values the axis labels are displaying as 0.01 instead of 1%.
* Bug Fix: Custom markers in export to PDF are appearing smaller in size than in the dossiers.
* Bug Fix: Data markers are not displaying in mobile
