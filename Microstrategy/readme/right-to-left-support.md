# Right-to-left Support

\


### Right to Left (RTL) Language Support <a href="#right-to-left-rtl-language-support" id="right-to-left-rtl-language-support"></a>

Vitara Charts supports scripts written from right to left. Arabic, Hebrew, Persian/Farsi, and Urdu are among the languages that utilize right to left scripts.

#### Controlling the option <a href="#controlling-the-option" id="controlling-the-option"></a>

The use of RTL is a system-wide option. It will be reflected on all Vitara charts once we activate it. Take note of the following line in the ‘global.txt’ file:

By default, the option is commented out. Simply remove the ‘#’ character from the preceding line to enable RTL data display.

#### Grid and Micro Charts <a href="#grid-and-micro-charts" id="grid-and-micro-charts"></a>

RTL format is commonly used in grid and micro charts. The following adjustments were done to Grid/Micro charts in order to properly support RTL format:

Headers: Attributes will be listed on the right side of the grid, while metrics will be listed on the left.

Context menu - Text order and indication arrows ‘>’: The text appears on the right side, while the arrow option appears on the left.

By default, all columns (including grouped column text) are right justified.

Threshold values have markers to the right of the marker and values to the left of the marker.

Threshold bars are ordered from right to left (vertical axis on the right).

Trend lines in micro charts begin on the right (for all; bar, column, and bullet).

Manage column group menu now have draggable elements on the right and the drop area is on the left.

#### Cartesian Charts <a href="#cartesian-charts" id="cartesian-charts"></a>

By default, the horizontal axis in all cartesian charts will grow from right to left. The vertical axis remains the same (it grows from bottom to top).

#### Grid layout Charts <a href="#grid-layout-charts" id="grid-layout-charts"></a>

For charts that use a grid layout (like the waffle, trellis, etc.), the layout will start from the top right instead of top left.

#### Properties Editor <a href="#properties-editor" id="properties-editor"></a>

The headers are now on the right (with the arrow key indicating selection on the left of the text), much like the context menu in the grid, and the content is on the left.

The label and the control (such as a checkbox, select box, etc.) will be switched for each of the properties. On the right will be the label or header, and on the left will be the control.

#### Legend <a href="#legend" id="legend"></a>

For all the legend elements (laid out horizontally), the symbols will be shown on the right and the text on the left.

#### Tooltip <a href="#tooltip" id="tooltip"></a>

The text will be right justified by default.
