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

`open RNTest.xcworkspace`

compile
