# Grid Custom CSS

From 4.4 version of Vitara Charts, users can customize grid chart by formatting the styles of rows and columns. Lets see those formattings below one by one.

#### 1. Row Styles: <a href="#id-1-row-styles" id="id-1-row-styles"></a>

**1.1 Styling all the rows**

Each row in the grid can be commonly styled using the below class.

```
.vitara-row{
    color:blue; 
    background-color:lightblue !important;
    font-family:calibri;
    font-size:14px; 
}
```

Below is the screenshot with the above custom styles applied.\
\


**1.2 Styling Even/Odd rows**

All the even rows in the grid can be styled using the below class

```
.vitara-row.vitara-grid-row-even{
    color:white;
    background-color: lightseagreen;
    font-size:12px;
    font-family:verdana;
}
```

All the odd rows in the grid can be styled using the below class

```
.vitara-row.vitara-grid-row-odd{
    color:wheat;
    background-color:teal;
    font-family:helvetica;
    font-size:12px;
}
```

Below is the screenshot which shows the applied styles for even and odd rows.\
\


#### 2. Grouped Row Styles <a href="#id-2-grouped-row-styles" id="id-2-grouped-row-styles"></a>

**2.1 Styling all the grouped rows**

To style all the grouped rows in the chart, use the below class.

```
.vitara-row.vitara-grid-row-group{
	color:indigo !important;
}
```

Below screenshot shows the above styles applied for the grouped rows.\
\


**2.2 Styling Even/Odd grouped rows**

All the even grouped rows in the grid can be styled using the below class

```
.vitara-row.vitara-grid-row-even.vitara-grid-row-group{
    color:orange;
    background-color:purple;
    font-family:lucida console;
    font-size:12px;
    font-weight:bold;
}
```

All the odd grouped rows in the grid can be styled using the below class

```
.vitara-row.vitara-grid-row-odd.vitara-grid-row-group{
    color:purple;
    background-color:orange;
    font-family:lucida console;
    font-size:12px; 
}
```

Below is the screenshot that shows the styles applied on odd and even grouped rows.\
\


The headers in the grid can be styled using the below class.

```
.vitara-header.vitara-grid-header-cell {
	color:brown;
	font-size:15px;
	font-family:calibri;
	font-weight: bold;
	background-color:pink;
}
```

Below screenshot shows the above styles applied on the header cell in the normal grid.\
\


Grouped header cells are formed by either pivoting or column grouping. These headers can be styled by using the below class. These styles will not be applied to the header cell in a normal(neither pivoted nor column grouped) grid.

```
.vitara-header.vitara-grid-grouped-header-cell{
	color:blue;
	background-color:silver;
}
```

Below screenshot shows the above styles applied on the grouped header cell.\
\


#### 4. Styling the Subtotals <a href="#id-4-styling-the-subtotals" id="id-4-styling-the-subtotals"></a>

Subtotal headers can be styled using the below class.

```
.vitara-grid-subtotals-header.vitara-grid-subtotals-cell{
    color:yellow;
    background-color:orange;
}
```

Below screenshot shows the above styles applied for the subtotal header.\
\


**4.2 Styling the Subtotal values**

Subtotal values can be styled using the below class.

```
.vitara-grid-subtotals-value.vitara-grid-subtotals-cell{
    color:yellow;
    background-color:orange;
}
```

Below screenshot shows the above styles applied for the subtotal values.\
\


#### 5. Column Styles <a href="#id-5-column-styles" id="id-5-column-styles"></a>

Every even column can be styled using the below class.

```
.vitara-grid-column:nth-child(2n){
	color:#ff890f;
	background-color:#0ff888;
 	font-weight:bold;
	font-family:verdana;
	font-size:11px;
}
```

Every odd column can be styled using the below class.

```
.vitara-grid-column:nth-child(2n+1){
	color:#fff;
	background-color:#ff8800;
	font-size:11px;
	font-family:verdana;
}
```

Below is the screenshot that shows the applied styles for odd and even columns.\


The styles applied for columns will also be reflected for Grand totals, to overcome those we will style grand totals using the below classes

```
.vitara-grand-totals-header.vitara-grand-totals-cell{
	color:red;
	background-color:black;
}
.vitara-grand-totals-value.vitara-grand-totals-cell{
	color:red;
	background-color:black;
	font-weight:unset;
}
```

See the screenshot below which shows the grand total styles that overcomes the column styles applied on it\
\


#### 6. Grand Totals <a href="#id-6-grand-totals" id="id-6-grand-totals"></a>

**6.1 Grand totals row**

The entire grand totals row can be styled using the below class

```
.vitara-grand-totals.vitara-grand-totals{
    color:white;
    background-color:brown !important;
    font-family:lucida console;
    font-weight:bold;	
}
```

See the below screenshot with the above properties applied.\
\


**6.2 Grand totals title**

To style only the grand totals title, use the below class

```
.vitara-grand-totals-header.vitara-grand-totals-cell{
    color:yellow;
    background-color:seagreen;
    font-family:helvetica;
    font-weight:bold;
    font-style:italic;
}
```

See the screenshot with the above properties applied only to the grand totals title.\
\


**6.3 Grand totals values**

To style only the grand totals’ values, use the below class.

```
.vitara-grand-totals-value.vitara-grand-totals-cell{
    color:lightgreen;
    background-color:teal;
    font-family:verdana;
    font-style:italic;
}
```

See the below screenshot with the above properties applied only to the grand totals values\
\


#### Custom themes <a href="#custom-themes" id="custom-themes"></a>

From 4.5 version of Vitara Charts, users can create their own themes and use those themes in Grid chart\
Two files in the VitaraCharts/custom/ folder are required to create custom themes. They are global.txt and customStyles.css.

The CSS class names and properties will be added to the customStyles.ccs file. Consult the sections 1 through 6 above to learn more about CSS classes and properties. Themes will be listed in the global.txt file in order to make them visible in the property editor.

**Step 1:**

For example, if we have to create a theme named ‘theme1’ which styles even and odd rows of the grid chart. Then in customStyles.css file, the format of CSS code should be as

```
.Theme1 .vitara-row.vitara-grid-row-even{
    color:white;
    background-color: lightseagreen;
    font-size:12px;
    font-family:verdana;
}
```

```
.Theme1 .vitara-row.vitara-grid-row-odd{
    color:wheat;
    background-color:teal;
    font-family:helvetica;
    font-size:12px;
}
```

The name of the theme is Theme1 in the code above. And, as you may have noticed, the theme name ‘Theme1’ is repeated, that is, the name appears in both the first and second pieces of code. According to the feature, the theme name should be repeated as many times as there are code blocks in order for certain styles to be applied solely to a single theme.

Let’s make another theme that styles all of the rows and header cells. Also, the format should be as follows:

```
.Theme2 .vitara-row{
    color:blue; 
    background-color:lightblue !important;
    font-family:calibri;
    font-size:14px; 
}
```

```
.Theme2 .vitara-header.vitara-grid-header-cell {
	color:brown;
	font-size:15px;
	font-family:calibri;
	font-weight: bold;
	background-color:pink;
}
```

And in the above blocks of CSS code also, the theme name Theme2 is repeated.

**Step 2:**

Now, add those theme names to the global.txt file in the way shown below. Please keep in mind that theme names are case sensitive. As a result, the names should be the same as they are in customStyles.css.

```
gridThemes.themes=Theme1,Theme2
```

The themes will then be listed in the grid chart. This can be verified in two ways: one using the property editor and the other through the context menu \[2020]. Please see the screenshots below.

1. Property Editor\

2. Context menu\


**Step 3:**

Now, apply Theme1 from either the property editor or context menu. Then the charts like below screenshot.\


And apply Theme2. Then the chart looks like the screenshot below.\


**Base Themes**

The base theme is the one to which custom theme styles are applied. A custom theme is always applied to a base theme. For example, we have a grid chart with the subject ‘Blue’. And now, when we apply a custom theme, the styles are applied to a white-based theme rather than a blue-based theme. This is due to the fact that all custom themes are by default based on the white theme.

The grid chart saved with the ‘Blue’ theme is shown below in a screenshot.&#x20;

After applying the custom theme ‘theme1’, the base theme gets changed to white. See the colors of headers and group dropzones in the below screenshot.\


**Changing the base theme:**

The basic theme for custom themes can also be changed. The starting point might be an in-built theme or any customised theme. For example, if we want the default theme to be ‘Dark,’ add the following line to the global.txt file.

```
gridThemes.baseThemes=Dark
```

Apply the custom theme ‘Theme1’ now, and the styles will be applied to the ‘Dark’ base theme. Compare the screenshot below to the previous screenshot.&#x20;

**Setting default theme**

We can now set the Grid chart’s default theme as of Vitara Charts version 4.5. A built-in theme or a custom theme can be used as the default theme. For instance, if we want to make ‘Theme2’ a custom theme as the default theme, we would add the following to the global.txt file.

```
gridThemes.defaultTheme=Theme2
```
