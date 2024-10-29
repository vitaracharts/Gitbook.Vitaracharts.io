---
hidden: true
---

# License deployed but still getting an error

### **I’ve replaced the license file but it is not being read** <a href="#ive-replaced-the-license-file-but-it-is-not-being-read" id="ive-replaced-the-license-file-but-it-is-not-being-read"></a>

Please restart the web server after deployment of Vitara charts. Additionally browser caches need to be purged and a new session needs to be started. If issue persists, use the following link (after substituting your server and port numbers) to check if the license key was replaced correctly and compare it with the key provided to you.

```
https://<server>:<port>/MicroStrategy/plugins/VitaraCharts/license.txt
```

If you notice any unrecognizable character in the beggining of the file (as displayed in the browser), you should make sure that character is removed. You can just copy the contents without the character and paste it back into your license file. Then retry loading the document/dashboard.

If the issue is still unresolved, please contact support.vitaracharts@vitara.co with details of the version, web server, steps taken and license key used for our tech support team to troubleshoot.

Last updated 22 days ago
