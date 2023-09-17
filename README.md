# ApexOracle_AuthSocial
Référence d'utilisation de Markdown [^1].   
Oracle APEX - How to Access Oracle APEX Applications With Google Credentials [^2].  
(A few details differents, that it is why all the pics)  
https://developers.google.com/identity/protocols/oauth2/  

**This tutorial have two mains part:**   
- Google console, to create a Auth Key  
- Config Apex Authentication Scheme  

  [Link to the project Apex Google Authentication](https://apex.oracle.com/pls/apex/r/cristianflc3/authentication-demo/)
  ![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/2a86f9ea-a2c9-46ac-adc4-1801eba79d44)

  <img src="https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/2a86f9ea-a2c9-46ac-adc4-1801eba79d44" width="500">

  
# 1 - Google console, to create a Auth Key  

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


# 2 - Config Apex Authentication Scheme  
  
### Go to Apex Workspace Utilities
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/86d2675f-2ced-4657-a3c5-1ac33a2b8baa)  

#### Then to Web Credentials  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/98a35f4c-12ff-4896-9b77-957187b9dbf1)  

#### Create  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/cd0e48f7-0713-4b94-969a-5f13fbbeaf38)  

### Add the parameters from the credencial  we created in google console (Client ID and CLient Secret)  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/b3a30e12-f1b9-4295-a32d-8de8f57f18de)   

#### Confirm the web credentials created
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/f071e620-f0c7-42ef-b48f-1b924855f6ed)  

### Go to your App, Share Components, Authentication Schemes  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/e79bb595-d3e8-4476-9efc-b9d25944837d)  

#### Create a Authentication Scheme
- Select the firts option, Based on a pre-configured scheme from the gallery  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/d35a4281-0705-4db1-a716-2b991e480071)   

#### Add the parameters    
Name,   
Scheme Type,   
Credential Storez, Select the one that we created in the previews steps  
Authentication Provider, select Google  
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/df2aa4cc-5ba0-4f41-a310-9d215a64fa2d)  
  
#### One last modification   
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/69334307-8a21-44ee-a37b-620086d553eb)   
  
#### Ajust one last parameter  
URL: https:// www.google.com/accounts/Logout   
![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/e2884a40-00aa-46c2-844b-7a58a51738f7)  
  
## Best part, the finist project  
https://apex.oracle.com/pls/apex/r/cristianflc3/authentication-demo/  

![image](https://github.com/Cristianfllc3/ApexOracle_AuthSocial/assets/72107370/83771c65-b3b5-4310-a9ec-350aaff8627b)  


Mercy, Thanks, Gracias, Gratie

  
[^1]:https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet.
[^2]:[https://www.youtube.com/watch?v=QJw4HkagVWc](https://www.youtube.com/watch?v=cK_aWXDVf_U&t=74s)https://www.youtube.com/watch?v=cK_aWXDVf_U&t=74s
