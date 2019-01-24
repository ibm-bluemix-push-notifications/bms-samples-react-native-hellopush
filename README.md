# bms-samples-react-native-hellopush

IBM Cloud push notifications service sample app in React native 


## Requirements:

- Xcode 10+
- Android: minSdkVersion 16+, compileSdkVersion 28+
- React Native >= 0.57.8
- React Native CLI >= 2.0.1

## Dependencies,

### iOS

#### Carthage 

1. Create a cart file inside the iOS app folder. Carthage file should be like this ,

```
github "ibm-bluemix-mobile-services/bms-clientsdk-swift-push"
```  

2. Do the `carthage update` in terminal.

3. open the Project in XCode and add the frameworks inside the `Embedded Binaries`

#### Add dependencies framework directly .

1.  Drag and drop the [BMSPush.framework](https://github.com/ibm-bluemix-mobile-services/bms-clientsdk-swift-push), [BMSCore.framework](https://github.com/ibm-bluemix-mobile-services/bms-clientsdk-swift-core) and [BMSAnalyticsAPI.framework](https://github.com/ibm-bluemix-mobile-services/bms-clientsdk-swift-analytics-api) to the iOS app.


### Android 

Create a [firebase project](https://console.firebase.google.com) and add the following bundle ids for android,

1. Add `com.bmdpush.react` and `com.ibm.mobilefirstplatform.clientsdk.android.push` .

Download the `google-services.json` and add inside the `node_modules` ➜ `bmd-push-react-native`  ➜ `android`.


## Usage

### Initialization

Open the `index.js` file and change the  `appGUID`, `clientSecret` and `region` . 


## Run

 To run the android , use the following ,
 
 ```
 $ react-native run-android
```

To run iOS open the `iOS` part in Xcode and run in your device. 



### Samples & videos

* Please visit for samples - [Github Sample](https://github.com/ibm-bluemix-mobile-services/bms-samples-android-hellopush)

* Video Tutorials Available here - [Bluemix Push Notifications](https://www.youtube.com/channel/UCRr2Wou-z91fD6QOYtZiHGA)

=======================
Copyright 2019 IBM Corp.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

