# React Native

### node.js
```angular2html
https://nodejs.org/ko/download/ - node-v14.15.1-x64.msi
```

### Android Studio
checked: Android SDK, Android SDK Platform, Android Virtual Device  
Environment Variables... - New... - User variables…  
JAVA_HOME: C:\Program Files\Android\Android Studio\jre\jre  
ANDROID_HOME: C:\Users\pc\AppData\Local\Android\Sdk  
PATH: %JAVA_HOME%\bin  
PATH: %LOCALAPPDATA%\Android\Sdk\platform-tools
```angular2html
$ java -version
openjdk version "1.8.0_242-release"
OpenJDK Runtime Environment (build 1.8.0_242-release-1644-b01)
OpenJDK 64-Bit Server VM (build 25.242-b01, mixed mode)
```

## Expo Cli
```angular2html
$ npm install -g expo-cli
$ expo init expocli
…
- cd reactnativeExpo
- npm start # you can open iOS, Android, or web from here, or run them directly with the commands below.
- npm run android
- npm run ios # requires an iOS device or macOS for access to an iOS simulator
- npm run web

$ cd expocli
$ expo start
```

### React Native Cli
```angular2html
$ npx react-native init reactnativecli
                  Welcome to React Native!
                 Learn once, write anywhere

√ Downloading template
√ Copying template
√ Processing template
√ Installing dependencies

Run instructions for iOS:
    • cd "C:\Users\pc\source\repos\reactnativecli" && npx react-native run-ios
    - or -
    • Open reactnativecli\ios\reactnativecli.xcodeproj in Xcode or run "xed -b ios"
    • Hit the Run button

  Run instructions for Android:
    • Have an Android emulator running (quickest way to get started), or a device connected.
    • cd "C:\Users\pc\source\repos\reactnativecli" && npx react-native run-android

  Run instructions for Windows and macOS:
    • See https://aka.ms/ReactNative for the latest up-to-date instructions.

$ cd C:\Users\PC\Documents\source\repos\reactnativecli
$ npx react-native run-android
```

### Error
```angular2html
java.lang.NoClassDefFoundError: Could not initialize class org.codehaus.groovy.vmplugin.v7.Java7
$PROJECT_ROOT/gradle/wrapper/gradle-wrapper.properties
…
distributionUrl=https\://services.gradle.org/distributions/gradle-6.3-bin.zip
# gradle Version: 6.3
$ run ./gradlew clean build
```

```angular2html
Failed to install the app. Please accept all necessary Android SDK licenses using Android SDK Manager: "$ANDROID_HOME/tools/bin/sdkmanager --licenses". Run CLI with --verbose flag for more details.
Android SDK – SDK Tools – [v] Google Play Licensing Library
or
Windows)
$ cmd.exe /C"%ANDROID_HOME%\tools\bin\sdkmanager.bat --licenses"
MacOS)
$ yes | $ANDROID_HOME/tools/bin/sdkmanager –licenses
```

### Modifying your app: App.js
