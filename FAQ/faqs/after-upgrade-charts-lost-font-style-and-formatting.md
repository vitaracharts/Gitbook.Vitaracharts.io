---
hidden: true
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

# After upgrade charts lost font style and formatting

Prior to 4.2 font sizing was a little inconsistent and too small to be readable in most circumstances. In the 4.2 release version the styling in vitara charts is modified. Due to this the charts created 4.1 or prior version does not look the same when we open in 4.2 or above versions.

However, there is an easy way to revert to the old defaults.

Open customStyles.css located in **VitaraCharts/custom** folder. As shown below there is a section specifically available to revert to 4.1 styles.

You’ll have to just uncomment this section. For uncommenting, remove the leading /\* mark and the last \*/ mark as shown below.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
