---
hidden: true
---

# How can I handle URLs in Vitara Charts globally?

#### How can I enable or disable URLs in Vitara Charts globally? <a href="#how-can-i-enable-or-disable-urls-in-vitara-charts-globally" id="how-can-i-enable-or-disable-urls-in-vitara-charts-globally"></a>

To control URLs globally, update the global.txt file:

* Path for MSTR Web Application: webapps\MicroStrategy\plugins\VitaraCharts\custom
* Path for MSTR Library Application: webapps\MicroStrategyLibrary\plugins\VitaraCharts\custom

**Add the property:**

security.allowURLLinks = 0 or 1

* 0 - URLs are disabled (default setting).
* 1 - URLs are enabled.

**How can I enable or disable URLs for individual charts?**

In each chart’s properties window:

* Go to the “Security” tab.
* Set Allow URL Links to Default (follows global.txt settings), Enable, or Disable for that specific chart.

**What happens if I don’t configure URL settings?**

If neither the global.txt file nor individual chart settings are configured, all URLs in VitaraCharts will be blocked by default.

**Handling Relative URLs**

For XSS protection, ensure relative URLs in href or src attributes start with a forward slash (/). This is required for proper encoding.

For more details, please refer to the Vitara Charts URL Security Documentation[https://docs.vitaracharts.com/guideCommonFeatures/allowURLs.html](../readme/allow-block-urls.md)
