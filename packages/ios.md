# iOS

For iOS you need to install Xcode which is about 2GB.

##Running on an iOS simulator (Mac Only)

If you have a Mac, you can run your app inside the iOS simulator.

Go to your app folder and type:

```unix
meteor install-sdk ios
```
This will run you through the setup necessary to build an iOS app from your project. When you're done, type:
```unix
meteor add-platform ios
meteor run ios
```
You will see the iOS simulator pop up with your app running inside.

##Running on an iPhone or iPad

*(Mac Only; requires Apple developer account)

If you have an Apple developer account, you can also run your app on an iOS device. Run the following command:

```unix
meteor run ios-device
```
This will open Xcode with a project for your iOS app. You can use Xcode to then launch the app on any device or simulator that Xcode supports.

If you want to point your app at the previously deployed server, run:
```unix
meteor run ios-device --mobile-server my_app_name.meteor.com
```
Now that we have seen how easy it is to deploy our app and run it on mobile, let's get to adding some more features.
