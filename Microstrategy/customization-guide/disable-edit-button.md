# Disable Edit button

\


## Hide ‘Edit’ button <a href="#hide-edit-button" id="hide-edit-button"></a>

Users can modify Vitara Charts by using the properties box that appears when we click the ‘Edit’ button. Vitara charts will display this ‘Edit’ option when the user hovers the cursor over any of the charts. By deactivating the ‘Edit’ option, we may prevent end users from making changes after the dashboard designer has completed his or her work.

## VI Dashboards or Dossiers <a href="#vi-dashboards-or-dossiers" id="vi-dashboards-or-dossiers"></a>

When the VI Dashboard/Dossier is run in “Presentation Mode,” the Vitara Charts do not display the ‘Edit’ button.

## Report Services Documents <a href="#report-services-documents" id="report-services-documents"></a>

In MicroStrategy, the concepts of “User Privileges” and “File Permissions” are used to implement security at various levels of users. Vitaracharts can be configured using the security model so that only developers or document designers, not end users, can change the Vitara charts. Depending on the privileges or file permissions that a user has in MicroStrategy, we can allow or limit a user from editing or modifying Vitara charts.

## **Disable edit button using User Privileges:**

The privilege and permission settings in Vitara Charts are configured in the ‘global.txt’ file, which is located in the Vitara Charts installation folder. In general, it will take the following path:

```
Tomcat 8.0\webapps\MicroStrategy\plugins\VitaraCharts\custom.
```

In the ‘global.txt’ file, the code “#checkPrivilegeForPropertiesEditor=125” will handle user privileges. In this line, we must specify the DSSXML Privilege value of the privilege on which we want to impose a security requirement. The DSSXML Privilege value of ‘Web Document Design’ is 125 by default. Uncomment this line by removing the ‘#’ to establish the criteria ‘Web Document Design’ using user privilege. Only users with the ‘Web Document Design’ privilege will now be able to edit all Vitara charts. You can also use additional privileges to set this requirement. The DSSXML permission value for the ‘Web Print Mode’ permission, for example, is 27. In the privilege settings line, enter these values.

```
checkPrivilegeForPropertiesEditor=27 
```

The users with this privilege enabled are only able to edit or modify Vitaracharts.

## **Disable edit button using File Permissions:**

Vitara Charts will inherit a user’s file permissions on a specific report services document and display the ‘Edit’ button if they match the permissions provided in the global.txt file. The following code will deal with setting security conditions applying file permissions in the ‘global.txt’ file.

```
#accessControlLevels=read/write
```

This line will be commented by default. Remove the ‘#’ character to uncomment this line. If you only want people with ‘Write’ permission on a certain document to be able to change Vitara charts, adjust the code as follows.

```
accessControlLevels=write
```

Now only the users who have to write permission on that particular report services document will get the ‘Edit’ button in Vitara Charts.
