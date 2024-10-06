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

# Workstation import visualization error

When we try to import custom visualizations in MicroStrategy Workstation, we sometimes get an error message -**Custom visualization import failed. Please select the correct file”**.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

This issue occurs when the user who is currently signed in to the computer does not have administrative access to the installation folder for the MicroStrategy Workstation. On a Windows computer, you can typically find this folder at the path mentioned below.

_C:\Program Files\MicroStrategy_

Step:1 In order to fix this problem, kindly follow the procedures below. Right-click on the workstation folder and select ‘Properties’.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

Step:2 Open the “Security” tab in the Properties window.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

Step:3 In the “Group or user names” pane select the user name with which you currently logged into the machine.

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

Step:4 The permissions that the user presently holds on the folder “Workstation” are displayed in the “Permissions for Users” pane.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

Step:5 An error relating to custom visualizations on the workstation is displayed when a user doesn’t have the “Modify” and “Write” permissions on the “Workstation” folder. We must provide the user with certain access in order to remedy this problem. Click on the “Edit button.

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

Step:6 In the “Permissions” window select the proper user name in the “Group or user names” pane and enable the check box “Allow” for the “Full Control” property.

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

Step:7 Click “Apply” and then click on “OK”.

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Step:8 Re-check; Right-click the “Workstation” folder, choose “Properties” from the menu, and then pick the “Security” tab to double-check that the proper user has been granted the proper permissions. Choose the user that is presently logged onto your computer. You can now see that the user has Full Control, Modify, and Write permissions enabled.

\


<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

Now try importing the custom VitaraCharts visualizations into the MicroStrategy Workstation application on your computer. The import of the custom visualizations will go well.
