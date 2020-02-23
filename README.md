# eduroam-wifi-Universidad-Politecnica-de-Madrid-UPM
Configuration of the netctl profile so you are able to connect to the UPM's eduroam wifi.
Tested in Arch, not using NetworkManager package.
1. Download the installer (script wrote in python, so you will have to download python 3/2 and python-distro)

 >http://www.upm.es/UPM/ServiciosTecnologicos/wifi?id=e83fe60106778110VgnVCM10000009c7648a____&fmt=detail
 
2. Run the scrip and follow the instructions:
    User name and password.
    
    When it asks you whether to make a wpa_supplicant file, write Y (yes).

3. Look for folder made by the script, if you have run it with:
  >sudo python3 .../eduroam-linux-UPdM.py

  The __ca_cert__ file and the __wpa_supplicant.conf__ will be put in: 
```  
/root/.cat_installer
        |----> ca.pem //ca_cert
        |
        |-----> cat_installer.conf // conf file
```
4.- Just copy the data and paste it into you netctl profile.

5.- I've left my netctl profile of eduroam in the repository.
