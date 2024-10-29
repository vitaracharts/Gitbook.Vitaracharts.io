---
hidden: true
---

# Secure Vitara license file

#### How to protect VitaraCharts license on the network and allow access to specific users <a href="#how-to-protect-vitaracharts-license-on-the-network-and-allow-access-to-specific-users" id="how-to-protect-vitaracharts-license-on-the-network-and-allow-access-to-specific-users"></a>

By default access to the vitara license from client browsers is left open using a URL of the format below.

http://host\_name:port/MicroStrategy/plugins/VitaraCharts/license.txt

However, access to the vitara license can be blocked by implementing the security constraints in the web.xml file. The web.xml file will be available in the following directory.

/\<Webserver>/webapps/MicroStrategy/WEB-INF/

Edit the **web.xml** file and copy and paste the below given security constraint just before the closing \</web-app> tag.

```
  <security-constraint>
          <display-name>Security constraint for Vitara license</display-name>
          <web-resource-collection>
              \** <web-resource-name>Protected Area</web-resource-name> \** 
              <url-pattern>/plugins/VitaraCharts/license.txt</url-pattern>
          </web-resource-collection>
          <auth-constraint>
              <!--uncomment role-name to allow access for specific roles-->
              <!-- <role-name>admin</role-name> -->
          </auth-constraint>
          <user-data-constraint>
              <transport-guarantee>NONE</transport-guarantee>
          </user-data-constraint>
  </security-constraint>
```

At this point, the file is not accessible to any user. Now you need to make sure the right role still has access to this file

* Uncomment the role-name tag in the auth-constraint section
* Replace “admin” with the right tomcat role corresponding to your MicroStrategy Web application deployment.

Save and close the **web.xml** file and restart the webserver.

For your reference, below is the screenshot of the **web.xml** file after adding the above security constraint code.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>
