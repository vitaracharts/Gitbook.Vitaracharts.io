# Condensed Metric Format

\


### Metric suffixes used to shorten high numbers in axis labels and data labels <a href="#metric-suffixes-used-to-shorten-high-numbers-in-axis-labels-and-data-labels" id="metric-suffixes-used-to-shorten-high-numbers-in-axis-labels-and-data-labels"></a>

Vitara charts will minimize the number in axis and data labels. The shortened metric suffixes can be changed to meet the needs of the user.

This can be accomplished by including the following code in the ‘global.txt’ file. The ‘global.txt’ file will be found in the Vitara charts plugin folder. Vitara charts → Custom folder → global.txt.

```
#Metric suffixes used to shorten high numbers in axis labels.
#empty-value, space, null is discarded.
shortFormatSymbols=k, M, B, T, P, E
```

In the preceding code, ‘k’ represents the suffix for 1000, M represents the suffix for 1000,000, B represents the suffix for 1,000,000,000, and so on. We can edit the suffix character in Vitara Charts to suit our needs.

For example, the value 1, 000, 000, 000  is automatically shortened as 1B. If we want to alter the suffix ‘B’ to another character, like ‘G,’ we must replace ‘B’ with ‘G’ in the above code.

```
shortFormatSymbols=k, M, G, T, P, E 
```

Save the ‘global.txt’ file and reopen your document. The below screenshot shows the new suffix ‘G’.

Note: If you still see the older suffix after reloading the dashboard, clear your browser’s cache and reload the dashboard.
