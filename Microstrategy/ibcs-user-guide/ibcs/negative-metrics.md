# Negative Metrics

\


#### Mapping metrics as negative <a href="#mapping-metrics-as-negative" id="mapping-metrics-as-negative"></a>

By default, all metrics are regarded as positive; that is, any positive change in the metric value (increase) is regarded as ‘good’ and is depicted in green (the default color). Obviously, there are some metrics (such as expenses) where a rise should be viewed negatively. These metrics should be labelled as such in the setting. This setup is currently done in the IBCSglobal.txt file.

\
The relevant section of the file looks like this:

```
#Support for negative metrics. Add metric names separated by comma
#negativeMetrics=AC
```

To add new metric names that should be viewed negatively,

*   Remove the leading # mark from the line (the # mark turns the line into a comment, which means it will not be read for system configuration purposes). The line now appears to be

    ```
    #Support for negative metrics. Add metric names separated by comma
    negativeMetrics=AC
    ```
* add any name of the metric or a pattern (regular expression)
* each name and pattern should be separated by a comma
* while using regular expressions, the entire expression should be enclosed with \[].

For example, if you would like to indicate that all metrics with the phrase expense in them should be treated as ‘negative’, you will change the line to

```
#Support for negative metrics. Add metric names separated by comma
negativeMetrics=[.*expense.*]
```

If you would like to add a specific metric name like ‘miscellaneous costs’, the line would now be

```
#Support for negative metrics. Add metric names separated by comma
negativeMetrics=[.*expense.*], miscellaneous costs
```
