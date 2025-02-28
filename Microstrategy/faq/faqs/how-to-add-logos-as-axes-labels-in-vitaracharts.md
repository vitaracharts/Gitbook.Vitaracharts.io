# How to Add Logos as Axes Labels in VitaraCharts?

To add logos as axes labels in VitaraCharts, the dataset must include a column containing tags or links, as these SVG images (logos) will be triggered by the HTML tags or links specified in the attribute. The logos will automatically display on the chart once this column is included in the attribute.\
**Note**: The custom logo can only be applied to one attribute in either the category axis or the color by field to ensure proper alignment with the bar.

## **Example of Dummy Dataset:**

Below is a sample dataset with the necessary structure for adding logos as labels:

<figure><img src="../../.gitbook/assets/logo dataset.PNG" alt=""><figcaption></figcaption></figure>

Now, when dataset is being added we need to convert the 'IMG SRC' into an HTML tag format like this:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcIi55B7PbHj1M6MU2iJryIGVIJjpSeyLkNLu1dEwFzBZmLod43-biHIvET1bWJ8R9HU21R5BLp_UaHbO_hVOaBZf6ssf8fCjhW3ImynoBG7x0nnMVIm1UstZOs-BdEFQYlk6PYUA?key=HG8zy91NAlh2msPjWJsC0g" alt=""><figcaption></figcaption></figure>

In the dataset, you define the height and width of the logos, and these values should be applied as the font size in the editor menu. This ensures that the logos align correctly with the bars on the chart.

### **Key Steps:**

1. **Define Logo Dimensions**: Specify the height and width of the logos in the dataset.
2. **Adjust Font Size:** In the editor menu, set the font size to match the height and width values of the logos. This step is essential for proper alignment of the logos with the chart's bars.\
   ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpjydpFGILWViaGJ_nt2A7b48EvS-x9S56jLoNkqOjYzFxg8J_fG6DJJhnXt8KmZMR11cT--qdQfTrhs5c8TtFhBXL1rYfJ0yGEDddm-VUZudaWV_R33n4vdQT1kWhOJkk2ht8cw?key=HG8zy91NAlh2msPjWJsC0g)

By setting the font size according to the defined dimensions, the logos will align properly with the bars, ensuring a clean and accurate display.\
Here is the screenshot of the logos displayed with the Vitara Column chart.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfyYzpAD0JSF7z040R-P2gLwG8p3XHC-gUMyjemrqyeWWhKkKyGq5hQVGIE51lmNJD5nP2WW1naCnACCqlFUI1ZDkwp1tYXSeRxgXRT_32_y2hpxz28RShv-FaNdnh56kVwHQZ6yg?key=HG8zy91NAlh2msPjWJsC0g" alt=""><figcaption></figcaption></figure>
