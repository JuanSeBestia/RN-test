`react-native init RNTest`

`react-native info`

            info Fetching system and libraries information...
            System:
                OS: macOS Mojave 10.14.6
                CPU: (12) x64 Intel(R) Core(TM) i7-8850H CPU @ 2.60GHz
                Memory: 184.24 MB / 16.00 GB
                Shell: 5.3 - /bin/zsh
            Binaries:
                Node: 10.15.3 - /usr/local/bin/node
                Yarn: 1.19.1 - ~/.npm-packages/bin/yarn
                npm: 6.9.0 - ~/.npm-packages/bin/npm
                Watchman: 4.9.0 - /usr/local/bin/watchman
            SDKs:
                iOS SDK:
                Platforms: iOS 13.0, DriverKit 19.0, macOS 10.15, tvOS 13.0, watchOS 6.0
            IDEs:
                Android Studio: 3.4 AI-183.5429.30.34.5452501
                Xcode: 11.0/11A420a - /usr/bin/xcodebuild
            npmPackages:
                react: 16.9.0 => 16.9.0
                react-native: 0.61.2 => 0.61.2


`yarn add appcenter appcenter-analytics appcenter-crashes --exact`


Edit Podfile: adding use_frameworks!

``` ruby
target 'RNTest' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  use_frameworks!
```

`cd ios && pod install --repo-update`

```
Detected React Native module pods for appcenter, appcenter-analytics, and appcenter-crashes
Updating local specs repositories
Analyzing dependencies
Fetching podspec for `DoubleConversion` from `../node_modules/react-native/third-party-podspecs/DoubleConversion.podspec`
Fetching podspec for `Folly` from `../node_modules/react-native/third-party-podspecs/Folly.podspec`
Fetching podspec for `glog` from `../node_modules/react-native/third-party-podspecs/glog.podspec`
Downloading dependencies
Installing AppCenter (2.4.0)
Installing AppCenterReactNativeShared (2.4.0)
Installing DoubleConversion (1.1.6)
Installing FBLazyVector (0.61.2)
Installing FBReactNativeSpec (0.61.2)
Installing Folly (2018.10.22.00)
Installing RCTRequired (0.61.2)
Installing RCTTypeSafety (0.61.2)
Installing React (0.61.2)
Installing React-Core (0.61.2)
Installing React-CoreModules (0.61.2)
Installing React-RCTActionSheet (0.61.2)
Installing React-RCTAnimation (0.61.2)
Installing React-RCTBlob (0.61.2)
Installing React-RCTImage (0.61.2)
Installing React-RCTLinking (0.61.2)
Installing React-RCTNetwork (0.61.2)
Installing React-RCTSettings (0.61.2)
Installing React-RCTText (0.61.2)
Installing React-RCTVibration (0.61.2)
Installing React-cxxreact (0.61.2)
Installing React-jsi (0.61.2)
Installing React-jsiexecutor (0.61.2)
Installing React-jsinspector (0.61.2)
Installing ReactCommon (0.61.2)
Installing Yoga (1.14.0)
Installing appcenter (2.4.0)
Installing appcenter-analytics (2.4.0)
Installing appcenter-crashes (2.4.0)
Installing boost-for-react-native (1.63.0)
Installing glog (0.3.5)
[!] The 'Pods-RNTest' target has transitive dependencies that include statically linked binaries: (/Users/juansebestia/Documents/gits/RNTest/ios/Pods/AppCenter/AppCenter-SDK-Apple/iOS/AppCenterAnalytics.framework, /Users/juansebestia/Documents/gits/RNTest/ios/Pods/AppCenter/AppCenter-SDK-Apple/iOS/AppCenter.framework, /Users/juansebestia/Documents/gits/RNTest/ios/Pods/AppCenter/AppCenter-SDK-Apple/iOS/AppCenterCrashes.framework, and /Users/juansebestia/Documents/gits/RNTest/ios/Pods/AppCenterReactNativeShared/AppCenterReactNativeShared/AppCenterReactNativeShared.framework)
```

