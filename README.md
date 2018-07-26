

![React Native App](http://test-assets.surge.sh/app-atom.png)


## Create new react native app

```shell
>_ react-native init helloworld
 ```

* Updated the placeholder text to be conditional based on the platform
* Hello Apple and Apple logo appear on ios
* Hello Android and Android logo appear on android

## Notes on building react native app for ios

* Install X-Code and X-Code cli tools
* Carefully (!!) follow official react native tutorial to get started
  * https://facebook.github.io/react-native/docs/getting-started.html
  * select 'Building Projects with Native Code', your development OS, and ios

```shell
>_  react-native run-ios
 ```
* This takes a while the first time
* Opens simulator
* Starts Metro-bundler
* Puts app on the simulator screen
  * cmd-r to reload
  * cmd-d / shake for dev tools
* Unlike EXPO, does not re-bundle every time you save a module, need to press cmd-r in simulator.
* Like expo, rebundling is fast

### Putting the app on iphone
* Need apple developer account
  * Either get personal account ($99/year)
  * Or become a part of organization with enterprise account
* Open ios/helloworld.xcodeproj in XCode
* Select helloworld under TARGETS
* Identity: set a unique bundle identifier
* Signing: specify a developer account
* Connect iphone to the computer
* Select your phone as the device in the top navbar
* press play button to build and copy app on your phone


## Notes on building react native app for android

* Install Java JDK from official Oracle source
  * http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
* Carefully (!!) follow official react native tutorial to install Android Studio and related tools
  * https://facebook.github.io/react-native/docs/getting-started.html
  * select 'Building Projects with Native Code', your development OS, and Android
* Create and then launch a new virtual device (emulator)
  * details are in the above tutorial

```shell
>_  react-native run-android
```

### Putting the app on an android phone

* Make sure no virtual machines are running
* connect your android phone
* allow remote debugging from your computer
* rerun run-android command as before
