Similar to iOS, we must enable the correct permissions to use the Camera. 
Configure these in the AndroidManifest.xml file. Android Studio will likely open this file automatically, but in case it doesn't, locate it under android/app/src/main/.

<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />