## 😸 Poc Vonage

<p>Vonage Open Tok is a lib for Stream Video</p>
<br/>

## Tutorial for Vonage for RN

-> https://learn.vonage.com/blog/2020/10/12/build-a-video-conference-app-with-react-native-and-vonage-video-api/

## Install Vonage:

-> yarn add opentok-react-native

## React Native > 0.60

### IOS

-> Open <YourProjectName>.xcworkspace contents in XCode. This file can be found in the ios folder of your React Native project.

-> Click File and New File

-> Add an empty swift file to your project:

    You can name this file anything i.e: OTInstall.swift. This is done to set some flags in XCode so the Swift code can be used.

-> Click Create Bridging Header when you're prompted with the following modal: Would you like to configure an Objective-C bridging header?

-> Ensure you have enabled both camera and microphone usage by adding the following entries to your Info.plist file: (In your VsCode)

```bash
<key>NSCameraUsageDescription</key>
<string>Your message to user when the camera is accessed for the first time</string>
<key>NSMicrophoneUsageDescription</key>
<string>Your message to user when the microphone is accessed for the first time</string>
```

### Android

->Add the following to your project build.gradle file: (In your VsCode)

```bash
        maven {
            url "http://tokbox.bintray.com/maven"
        }
```

-> As for the older Android devices, ensure you add camera and audio permissions to your AndroidManifest.xml file: (In your VsCode)

```bash
    <uses-permission android:name="android.permission.CAMERA" />
    <uses-permission android:name="android.permission.MODIFY_AUDIO_SETTINGS" />
    <uses-permission android:name="android.permission.RECORD_AUDIO" />
    <uses-feature android:name="android.hardware.camera" android:required="true" />
    <uses-feature android:name="android.hardware.camera.autofocus" android:required="false" />
    <uses-feature android:name="android.hardware.microphone" android:required="true" />
```

Newer versions of Android–API Level 23 (Android 6.0)–have a different permissions model that is already handled by this library.

#### For more information:

-> https://github.com/opentok/opentok-react-native

---
