---
hidden: true
---

# Workstation import visualization error

When we try to import custom visualizations in MicroStrategy Workstation, we sometimes get an error message -**Custom visualization import failed. Please select the correct file”**. ![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_1.png)

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_2.png)

This issue occurs when the user who is currently signed in to the computer does not have administrative access to the installation folder for the MicroStrategy Workstation. On a Windows computer, you can typically find this folder at the path mentioned below.

_C:\Program Files\MicroStrategy_

Step:1 In order to fix this problem, kindly follow the procedures below. Right-click on the workstation folder and select ‘Properties’.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_4.png)

Step:2 Open the “Security” tab in the Properties window.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_5.png)

Step:3 In the “Group or user names” pane select the user name with which you currently logged into the machine. ![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_6.png)

Step:4 The permissions that the user presently holds on the folder “Workstation” are displayed in the “Permissions for Users” pane.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_7.png)

Step:5 An error relating to custom visualizations on the workstation is displayed when a user doesn’t have the “Modify” and “Write” permissions on the “Workstation” folder. We must provide the user with certain access in order to remedy this problem. Click on the “Edit button.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_8.png)

Step:6 In the “Permissions” window select the proper user name in the “Group or user names” pane and enable the check box “Allow” for the “Full Control” property.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_9.png)

Step:7 Click “Apply” and then click on “OK”.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_10.png)

Step:8 Re-check; Right-click the “Workstation” folder, choose “Properties” from the menu, and then pick the “Security” tab to double-check that the proper user has been granted the proper permissions. Choose the user that is presently logged onto your computer. You can now see that the user has Full Control, Modify, and Write permissions enabled.

![workstationError](https://vitaracharts.github.io/assets/img/faqs/workstationError\_11.png)

Now try importing the custom VitaraCharts visualizations into the MicroStrategy Workstation application on your computer. The import of the custom visualizations will go well.
