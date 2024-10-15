---
hidden: true
icon: book-open-cover
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

# Library

## [Click Here](https://vitarachartsdownloads.azureedge.net/distributions/Maps/5.2.0.499/VitaraMapsLibrary.zip)

You need to update the config path and point to the web server using the steps below. After extracting the VitaraMapsLibrary plugins into plugins folder of MicroStrategy Library server, navigate to the library configuration page:

```
https://<MicroStrategyLibraryServer>/plugins/VitaraMapsLibrary/config.jsp 
(ex: http://example.com/MicroStrategyLibrary/plugins/VitaraMapsLibrary/config.jsp)
```

Setting web configuration url to Vitara Maps config helps to render Vitara Maps chart without internet access to the ipad/iphone.

On the page enter the path to the **MicroStrategy Web application** (not library) and click submit.
