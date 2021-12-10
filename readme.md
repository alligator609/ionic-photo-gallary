Similar to iOS, we must enable the correct permissions to use the Camera. 
Configure these in the AndroidManifest.xml file. Android Studio will likely open this file automatically, but in case it doesn't, locate it under android/app/src/main/.

<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />


// change icon
First, install cordova-res:
npm install -g cordova-res
cordova-res expects a Cordova-like structure: place one icon and one splash screen file in a top-level resources folder within your project, like so:
resources/
├── icon.png
└── splash.png
Next, run the following to generate all images then copy them into the native projects:
cordova-res ios --skip-config --copy
cordova-res android --skip-config --copy
