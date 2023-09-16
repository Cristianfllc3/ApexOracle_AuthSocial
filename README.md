# ApexOracle_AuthSocial
Référence d'utilisation de Markdown [^1].   
Oracle APEX - How to Access Oracle APEX Applications With Google Credentials [^2].
(A few details differents, that it is why all the pics)

This tutorial have two mains part:    
- Google console, to create a Auth Key  
- Config Apex Authentication Scheme  

  ## Google console, to create a Auth Key  

### Create a project in console.developers.google.com (Apex Oracle Auth Social)  
https://console.cloud.google.com/apis/dashboard
  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/e1e6040e-7b84-49dd-abb2-2e7cef42b2dc)

### Go to Credentials, and create a : OAuth client ID  
    
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/e2395701-77e6-43c2-8bac-6bab6b6457be)


 ### In some cases it must, To create an OAuth client ID, you must first configure your consent screen
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/a67a6043-60c2-4fd1-8c1e-5db8dbb4943f)  
  
### Select external  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/d2206c37-17f6-402b-b3b3-d9b513fb04db)  

### Add this parameters:
#### APP DOMAIN
Aplication Home page:   
- https://apex.oracle.com/pls/apex/apex_authentication.callback  

#### AUTHORIZED DOMAINS:  
- oracle.com  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/9ac718dc-7351-49b2-9522-7f60caaf05e3)


###  Select the scope  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/68ccbd3a-bd18-4114-8eda-261221246ea5)  


### Add test users  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/0582894f-f805-407a-a7fc-24f070f9122b)  

### Now we can acces to create a OAuth client ID  
URIs: https://apex.oracle.com/pls/apex/apex_authentication.callback    
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/85368fe2-858e-4420-9614-9dd501fc0ebd)  

### Copy and Save, your Client Id and Client secret  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/7a403fed-20a7-461f-aacd-65736239616c)  


## Config Apex Authentication Scheme  
  


  
[^1]:https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet.
[^2]:[https://www.youtube.com/watch?v=QJw4HkagVWc](https://www.youtube.com/watch?v=cK_aWXDVf_U&t=74s)https://www.youtube.com/watch?v=cK_aWXDVf_U&t=74s
