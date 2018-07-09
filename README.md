## Working example for QRCode app

![](https://raw.githubusercontent.com/taboca/doc-js-example-qrcode-cam-example/master/doc/20180709_132010.gif)

This project is the result of an attempt to get a QRCODE scanner Android application working using React-native and the following packages:

* react-native-qrcode-scanner
* react-native-camera

Notice this was done in 9 July 2018. The purpose of this repository is to offer you an easy view about the changes that I had to do based on the initial state of a React-native application (the files produced by "react-native init MyApp"). Therefore this repository have only one major change:

## The initial code

The initial code refers to the files produced by the "react-native init YourAppName". You can see the initial code [here](https://github.com/taboca/doc-js-example-qrcode-cam-example/commit/c03e90476d7677dbf945c2687fe8b6e7e3f040e1).

## Packages installation changes

Once you have the initial React-native -based app, let's install the required packages dased in the documentation from [react-native-qrcode-scanner](https://github.com/moaazsidat/react-native-qrcode-scanner):

```
npm install react-native-camera --save
react-native link react-native-camera
npm install react-native-qrcode-scanner --save
react-native link react-native-qrcode-scanner
react-native link react-native-permissions
react-native run-android
```

## Patching gradle

[According to Upgrade gradle for Android Projects](https://github.com/react-native-community/react-native-camera/blob/master/docs/GradleUpgradeGuide.md) it' was necessary to patch the gradle infrastructure.

* [See all the file changes within the ./android](https://github.com/taboca/doc-js-example-qrcode-cam-example/commit/3594148e93e3ebf12f8d7530c3459e3cab92fe3a)
