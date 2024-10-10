# Vertical Waterfall

\


#### Vertical Waterfall chart <a href="#vertical-waterfall-chart" id="vertical-waterfall-chart"></a>

**Description**

This sort of chart is commonly used to display financial data over time. To compare performance, we allow you to create up to two of these waterfall charts (for two separate scenarios).

**Demo video**

**Scenario planning**

Please review mapping scenarios for a better understanding of how scenario planning in VitaraCharts.

For this type of chart, the scenarios are mapped using **attribute elements**. So the user will need to define metric values (for a set of metrics) for attribute elements representing different scenarios. For instance, if the user is looking to draw waterfalls for comparison for the years 2019 and 2018 where 2019 represents the actual data and 2018 represents the previous data, then

* the element 2018 should be mapped to Previous in the properties editor
* the element 2019 should be mapped to Actual

If instead, the user wants to compare 2019 performance against the plan, then the metric values need to be defined for 2019 and for 2019\_PL (this is just for illustration; the actual name of the element is up to the user) i.e the Year attribute should include both these attribute elements.

* the element 2019 should be mapped to Actual in the properties editor
* the element 2019\_PL should be mapped to previous
