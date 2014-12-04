# Android

Running on an Android emulator

In the terminal, go to your app folder and type:

```unix
meteor install-sdk android
```

This will help you install all of the necessary tools to build an Android app from your project. When you are done installing everything, type:

```unix
meteor add-platform android
```
After you agree to the license terms, type:

```unix
meteor run android
```
After some initialization, you will see an Android emulator pop up, running your app inside a native Android wrapper. The emulator can be somewhat slow, so if you want to see what it's really like using your app, you should run it on an actual device.

##Running on an Android device

First, complete all of the steps above to set up the Android tools on your system. Then, make sure you have USB Debugging enabled on your phone and the phone is plugged into your computer with a USB cable. Also, you must quit the Android emulator before running on a device.

Then, run the following command:

```unix
meteor run android-device
```

The app will be built and installed on your device. If you want to point your app to the server you deployed in the previous step, run:
```unix
meteor run android-device --mobile-server my_app_name.meteor.com
```
