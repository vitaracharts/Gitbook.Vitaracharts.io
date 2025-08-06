# Customization Tool

## Customization Tool Overview

A new interface has been introduced to simplify editing of key configuration files—global.txt, customStyles.css, and translation files—directly from within the system. This user-friendly tool removes the need for manual file edits, streamlining customization workflows.

**Available from Version 5.3.6**\
This release supports full editing of global.txt and translation files. Partial editing is available for customStyles.css, with full support planned for a future update.

### &#x20;Key Features

* Add and manage custom palettes
* Add and manage custom fonts
* Modify individual settings in global.txt
* Edit individual translated texts in translation files
* Switch between available languages

📌 **Note**: After configuring your settings, make sure to click Save Changes in the top-right corner.The changes will only reflect in the visualizations once this step is completed.

**Clear your browser cache** to ensure the updated customization appears correctly in the visualizations

\


<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDpy5QNGIHTa5oTkFoNxSBaJIhDBvykOw4ccYpaw4Su3AdjMeuPgTjmSc606gI6vQWHvhn94-6oLV6gKUO-NZA_IU0nefPjUFRDo4Pqf8r6tsfXH6EOTbCsl246I3wp4vRd0GT4w?key=GOHD-Vwdy0sntCqAMUofbw" alt=""><figcaption></figcaption></figure>

### Adding a Custom Palette

1. Enter a **name** for the new palette.
2. Click the **“+”** button to add and customize colors.
3. Click **Save Palette**.
4. Your palette will now appear in the saved list:

* **Enable it** using the checkbox.
* Use **Set as Default** if needed.\


5. Click **Save Changes** (top-right) to apply it to your charts.\
   To update an existing palette, click **Edit**, adjust the colors, and hit **Save.**\


### Define and Add a Custom Font

Ensure the font file is placed in the following directory:

* For **MSTR Web** : webapps\MicroStrategy\plugins\VitaraCharts\custom\fonts
* For **MSTR Library** : webapps\MicroStrategyLibrary\plugins\VitaraCharts\custom\fonts

**Note** : If the fonts folder does not exist under the custom directory, users can manually create it and then add your font files.

**Steps :**

**1. Enter Font Details**

* Specify the Font Name.
* Provide the source font file
* Click Add Font to save it. The font will now appear in the list of saved fonts.\


**2. Set the Font as Default**

To apply the newly added font as the default:

* Locate it in the Saved Fonts list.
* Enable the Set as Default option.

The selected font will now be used as the default across all  visualizations.

Refer to the attached GIF below for a demonstration of custom palette and custom font configuration.

<figure><img src="../.gitbook/assets/Doc customization.gif" alt=""><figcaption></figcaption></figure>

### Modifying global.txt Settings

Toggle individual settings within the tool to replicate the effects of manual edits to global.txt, presented in a more intuitive format.

### Refer to the attached screenshot for details.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXduM56sssc5Mn8Rj40VRJH-MRV0iaXicx7PFKtTnTYIh3bhFKNhN9FNJkkvU_tKRbV2u8nwkwX0oqZZfphDfk3eGkAs2cplAqwhTrhGktKs6cNKiswh8Pn41ifsMOGpZuTXDAkf9g?key=GOHD-Vwdy0sntCqAMUofbw" alt=""><figcaption></figcaption></figure>

### Translation&#x20;

The Translation tab allows users to:

* Edit individual entries in the translation files
* Switch between multiple language options

Below the screenshot for your reference\


<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcCGZAaak_BaLV_xBJfr_4iVxbBwYO1Bl3E31VeTlf_5BtHlyasif_Q7YoWxvTuXoq_lJ5xn1YhN-UclOrWvipjMtTgh9SuZkFxb53Z5WPNpD-QbM_Jn2XMQOF6nlZadvvFTBpEdw?key=GOHD-Vwdy0sntCqAMUofbw" alt=""><figcaption></figcaption></figure>

### File Access Path

Access the customization interface from the following locations:

* For MicroStrategy Web Application:\
  &#xNAN;**/MicroStrategy/plugins/VitaraCharts/utils/customizations.html**
* For MicroStrategy Library Application:\
  &#xNAN;**/MicroStrategyLibrary/plugins/VitaraCharts/utils/customizations.html**

📌 **Note**: Customizations must be applied separately for Web and Library environments

\
\
\
\
\
\
\
