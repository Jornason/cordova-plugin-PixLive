# Cordova plugin for PixLive SDK

This allows a seamless bridge for using Augmented Reality PixLive SDK into your own Cordova application.

Check [http://www.pixlive.info](http://www.pixlive.info) for more information and the Ionic plugin at [http://vidinoti.github.io/angular-pixlive/](http://vidinoti.github.io/angular-pixlive/)

## Installation
Create an account, obtain a licence and dowload SDKs at https://www.vidinoti.com/

Install the plugin by passing the VDARSDK.framework and vdarsdk-release.aar file of the PixLive SDK to the plugin installation command line:

```bash
cordova plugin add cordova-plugin-pixlive@latest --variable LICENSE_KEY=MyLicenseKey --variable PIXLIVE_SDK_IOS_LOCATION=\"path/to/VDARSDK.framework\" --variable PIXLIVE_SDK_ANDROID_LOCATION=\"path/to/android/vdarsdk-release.aar\"
```

## Cordova PixLive Demo App

* Create a new Cordova project using cordova-template-PixLive

```bash
cordova create myArApp com.mycompan.myArApp myArApp --template https://github.com/vidinoti/cordova-template-PixLive.git
```

* Add android and iOS platforms

```bash
cordova platform add android
cordova platform add ios
```

* Add the Cordova plugin for PixLive SDK to your project

```bash
cordova plugin add cordova-plugin-pixlive@latest --variable LICENSE_KEY=MyLicenseKey --variable PIXLIVE_SDK_IOS_LOCATION=\"path/to/VDARSDK.framework\" --variable PIXLIVE_SDK_ANDROID_LOCATION=\"path/to/android/vdarsdk-release.aar\"
```

* Build your project
```bash
cordova buil android
cordova build ios
```

* Test the app on an Emulator
```bash
cordova emulate android
cordova emulate ios
```
