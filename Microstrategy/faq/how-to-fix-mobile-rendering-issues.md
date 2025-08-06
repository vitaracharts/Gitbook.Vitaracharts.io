---
hidden: true
---

# How to fix mobile rendering issues?

#### Seeing a blank screen on mobile <a href="#seeing-a-blank-screen-on-mobile" id="seeing-a-blank-screen-on-mobile"></a>

## **1. Check your deployment**

This issue is typically caused by wrong configuration/deployment of charts.

First, please check to make sure the proper VitaraCharts plugin is deployed; In the case of mobile, the plugin to download is called VitaraChartsMobile.zip

Follow all the installation steps listed in the [install guide for mobile](https://docs.vitaracharts.com/install-docs/installing-on-microstrategy-mobile).

**Note** that after deploying, the plugins folder will have several Vitara related folders (one for each type of chart)

<figure><img src="../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

* In case a cluster of mobile servers are being used, it is critical to ensure Vitaracharts is deployed to all nodes in the cluster.
* Also please verify that the version of Charts deployed in Mobile and Web both are same.
* If you are using VitaraCharts for Documents please make sure that Display widget option in (iPhone, iPad,Android..etc) is enabled for the widget. \</br>

<figure><img src="../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

## **2. Clear mobile/library application cache**

You deployed charts correctly and still you are seeing a blank screen on mobile/library application in IOS or android device, please delete the chache of the application and reload the dossier/document. Generally, you need to do this when you deploy new vitara build or after Setting web configuration url to library/mobile application’s Vitara Charts config file.

### **To clear cache in the library application on iPad please follow the below steps:** ![Mobile Configuration Editor](https://docs.vitaracharts.com/assets/img/faqs/libraryIcon.jpg)

#### **Step 1:**

\


<figure><img src="../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>

#### Step 2:

<figure><img src="../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

#### Step 3:

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

#### Step 4:

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

### **To clear cache in the MicroStrategy mobile application on iPad please follow the below steps:**&#x20;

#### Step 1:

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

#### Step 2:

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

### Step 3:

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>
