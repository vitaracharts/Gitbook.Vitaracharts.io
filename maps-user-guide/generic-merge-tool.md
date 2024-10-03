# Generic Merge tool

Vitara’s Generic Merge Tool offers a powerful solution for creating custom grouped regions on geographical maps, allowing users to merge individual regions based on specified criteria. This guide walks you through the process of using the tool to generate CBSA (Core-Based Statistical Areas) regions using a geojson collection of US counties.

#### Embracing the Power of Vitara’s Generic Grouping Tool <a href="#embracing-the-power-of-vitaras-generic-grouping-tool" id="embracing-the-power-of-vitaras-generic-grouping-tool"></a>

Nestled within Vitara’s arsenal is the Generic Grouping Tool, a powerhouse capable of merging individual regions on a map into a singular, cohesive masterpiece. This tool derives its strength from a data file containing invaluable grouping information, weaving an intricate tapestry of insights.

To embark on this journey, navigate through the digital realm by following this enchanted link: [VitaraMaps - Tool for grouping features](https://cloud.vitaracharts.com/maptools/generic.html)

Behold, the following snapshot encapsulates the mystique of the Generic Grouping Tool’s web page:&#x20;

#### Example of generic aggregation: <a href="#example-of-generic-aggregation" id="example-of-generic-aggregation"></a>

Now, let’s dive into a practical example—creating CBSA regions using a geojson collection of US counties. Before diving into the tutorial, ensure that the VitaraMaps package is installed. Locate the US County level geojson file within the package at /plugins/VitaraMaps/custom/shapes/us-all-admin2.geo.json. Or Begin by acquiring the GeoJSON file for US States from the trusted source: [Highmaps.](https://code.highcharts.com/mapdata/)

After downloading, open the file to verify that it encompasses the requisite data corresponding to your Excel sheet. This step ensures alignment between the geographical information in the GeoJSON file and the data you aim to visualize.

**Step-by-Step Walkthrough:**

**Step 1: Convert Geojson to Topojson**

* Begin by visiting Mapshaper[ a powerful tool for transforming geojson files into the Topojson format.](https://mapshaper.org/\))
* Use the platform to upload your geojson file and seamlessly convert it to Topojson. Below screenshot shows mapshaper webpage.

**Step 2:**

Once you’ve successfully converted your geojson file to Topojson using mapshaper.org, the next step involves uploading and visualizing your data on the Generic Merge Tool webpage.Follow these straightforward instructions:

* On the Generic Merge Tool webpage, locate the “Select” button prominently displayed.
* Clicking on the “Select” button will prompt a file selection dialog. Navigate to the directory where you saved the geojson file on your local machine.
* Once you’ve chosen the geojson file, the webpage will dynamically display your uploaded file as an interactive map.

**Step 3:**

Subsequently, click on the “Export” button located at the top-left corner of the webpage on mapshaper.

**Step 4:**

Choose required/both the layers and set the file format to “TopoJSON”. Execute the export by clicking the designated button, as illustrated in the screenshot. This action will initiate the download of your newly created TopoJSON file.

**Step 5:**

Transition to the generic tool webpage and upload the TopoJSON file that you’ve just created. Follow the visual reference provided in the accompanying screenshot to guide you through this step.

**Step 6:**

To obtain the TopoJSON object name from the downloaded file, use jsonviewer.stack.hu. Follow these steps:

1. Open jsonviewer.stack.hu.
2. Paste the content of the downloaded TopoJSON file in the ‘Text’ tab. This process allows you to inspect the file structure and identify the specific TopoJSON object name needed for the next steps in the custom map generation. (https://docs.vitaracharts.com/guideMapFeatures/customizingMapChart.html)

**Step 7:**

Enter the TopoJSON object name that you’ve retrieved from the JSON viewer into the designated field. This ensures that the generic tool recognizes and utilizes the correct TopoJSON object for the subsequent stages of the custom map generation process.

**Step 8:**

In this step, you’ll integrate grouping information into the process by uploading a CSV file containing CBSA and FIPS codes.

* Ensure your CSV file is structured with columns corresponding to CBSA and FIPS codes, containing the relevant grouping information.
* Identify the designated data field on the Generic Merge Tool webpage where you’ll upload your CSV file.
* Click on the appropriate area, typically labeled “Upload” or “Browse,” to select your prepared CSV file from your local machine.
* Once selected, confirm the upload to integrate your CSV file into the tool.

**Step 9:**

In this step, you’ll specify the column on which the grouping will be performed.

* On the Generic Merge Tool webpage, identify the “Group By” field, where you’ll specify the column for grouping.
* Enter the column name on which the grouping is to be performed. In this example, use the CBSA column from your uploaded CSV file.

**Step 10:**

In this step, you’ll configure the Data Prop and Shape Prop fields, which play a crucial role in mapping features between the shapefile and data file.

* In the “Data Prop” field, enter the column name from your CSV file that contains the relevant data. In this example, it is the FIPS column.
* In the “Shape Prop” field, enter the column name from your Topojson file that corresponds to the data. In this case, it is the fips column. By configuring the Data Prop and Shape Prop fields correctly, you establish the link between the CSV file and the Topojson file. This alignment is crucial for the tool to intelligently merge and map the data, ensuring accuracy and consistency in your grouped regions.

**Step 11:**

Carefully fill in any remaining required information on the Generic Merge Tool webpage. Ensure all fields are populated with the relevant data, confirming accuracy.

* Click on the “Export” button to commence the merging process. The tool will intelligently merge the specified regions based on your configurations.
* Once the merging process is complete, the tool will generate and provide a link to download the merged Geojson file.

**Step 12:**

Congratulations on successfully downloading the merged Geojson file! The final step involves using this file to create a new map layer. Refer to the Creating New Map Layer[ documentation provided in the tool’s resources. This documentation will guide you through the process of incorporating your downloaded Geojson file into a new map layer.](https://docs.vitaracharts.com/guideMapFeatures/creatingNewMaps.html)

The image below captures the visual culmination of our efforts — a beautifully merged map showcasing the outcome of the grouping process. This output map file elegantly represents the amalgamation of regions based on the specified criteria, providing a comprehensive and visually appealing snapshot of the customized geographical data
