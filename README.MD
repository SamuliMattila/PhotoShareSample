﻿Photo Share Sample App
==============================
An event-based picture sharing app allowing users participating to a certain event to share related pictures, with real-time synchronization and automatic
categorization on the cloud based on the presence of people.

This app was made as mobile cloud computing course exercise. Code was written by Samuli Mattila,  Matias Hämäläinen and Daniele Magurano. Mayhaps it provides some inspiration for future generations. 


## Deploy instruction

To build the Android apk and deploy the backend application on Google Cloud Flexible Engine simply run the following command in the root directory:

```sh
$ ./deploy.sh
```

Then you can find the apk file to be installed in the following directory:

```  
android/app/build/outputs/apk/debug
```

Remember to change google cloud keys and access point to correspont your account.

## File and folder layout

    .
    ├── android
    │   ├── ...
    │   ├── app
    │   │   ├── ...
    │   │   └── src                                  # Android app source files
    │   │   ├── ...
    │   └── ...
    ├── backend                              
    │   ├── app.js                                   # Main backend application
    │   ├── app.yaml                                 
    │   ├── cron.yaml
    │   ├── ...
    ├── deploy.sh                                    # Deploy script
    └── README.MD