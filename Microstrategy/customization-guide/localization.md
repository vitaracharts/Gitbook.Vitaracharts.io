# Localization

These features are supported in the release 4.2 (or newer)

\


## How to add support for a new language <a href="#how-to-add-support-for-a-new-language" id="how-to-add-support-for-a-new-language"></a>

VitaraCharts editors are accessible in English, German, French, and Spanish out of the box. It is possible to add support for new local languages on your own. The steps are as follows:

*   Create a file MessageBundle\_\<languagecode>\_\<regioncode>.txt in directory /VitaraCharts/custom/

    ```
    Example: For “fr-fr” as user language, 
    file name should be: MessageBundle_fr_fr.txt
    ```
* Copy the content from file VitaraCharts/custom/MessageBundle\_en\_us.txt in newly created file (MessageBundle\_\<languagecode>\_\<regioncode>.txt)
*   Add the respective translation for English string separated by “=” operator

    ```
    Format: \<English_String\>=\<Translated_String\>
    Example: Cell=Zelle
    ```

## Preference Order for how lanugage resources are loaded <a href="#preference-order-for-how-lanugage-resources-are-loaded" id="preference-order-for-how-lanugage-resources-are-loaded"></a>

* Language with regional Code (MessageBundle\_fr\_fr.txt )
* Language Only (MessageBundle\_fr.txt )
* Default (MessageBundle\_en\_us.txt)

**NOTE** : If the translation for some keys are missing in the file then those keys will be displayed in English Language in the Property Editor
