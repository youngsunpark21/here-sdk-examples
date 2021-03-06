# HERE SDK 4.x (Lite, Explore & Navigate Edition) - Examples for Android, iOS and Flutter
![License](https://img.shields.io/badge/license-Apache%202-blue)
![Platform](https://img.shields.io/badge/platform-Android-green.svg)
![Language](https://img.shields.io/badge/language-Java%208-orange.svg)
![Platform](https://img.shields.io/badge/platform-iOS-green.svg)
![Language](https://img.shields.io/badge/language-Swift%205.1.2-orange.svg)

The [HERE SDK](https://developer.here.com/products/here-sdk) enables you to build powerful location-aware applications. Explore maps that are fast and smooth to interact with, pan/zoom across map views of varying resolutions, and enable the display of various elements such as routes and POIs on highly customizable map views.

<center><p>
  <img src="images/here_sdk.jpg" width="500" />
</p></center>

The HERE SDK consumes data from the [HERE Platform](https://www.here.com/products/platform) and follows modern design principles incorporating microservices and highly modularized components. Currently, the HERE SDK supports three platforms: Android, iOS and Flutter.

For an overview of the existing features, please check the _Developer's Guide_ for the platform of your choice. Here you will also find numerous code snippets, detailed tutorials, the _API Reference_ and the latest _Release Notes_:

- HERE SDK for Android ([Lite Edition](https://developer.here.com/documentation/android-sdk/dev_guide/index.html), [Explore Edition](https://developer.here.com/documentation/android-sdk-explore), [Navigate Edition]( https://developer.here.com/documentation/android-sdk-navigate))
- HERE SDK for iOS ([Lite Edition](https://developer.here.com/documentation/ios-sdk/dev_guide/index.html), [Explore Edition]( https://developer.here.com/documentation/ios-sdk-explore), [Navigate Edition]( https://developer.here.com/documentation/ios-sdk-navigate))
- HERE SDK for Flutter ([Explore Edition](https://developer.here.com/documentation/flutter-sdk-explore), [Navigate Edition](https://developer.here.com/documentation/flutter-sdk-navigate))

> For now, the _Navigate Edition_ is only available upon request. Please contact your HERE representative to receive access including a set of evaluation credentials.

## List of Available Example Apps (Version 4.4.0.2)
In this repository you can find the latest example apps that show key features of the HERE SDK in ready-to-use applications:

- **HelloMap**: Shows the classic 'Hello World'.
- **HelloMapWithStoryboard**: Shows the classic 'Hello World' using a Storyboard.
- **Gestures**: Shows how to handle gestures.
- **MapMarker**: Shows how to add POI marker to the map.
- **MapObjects**: Shows how to add circles, polygons and polylines to the map.
- **MapOverlays** / **MapViewPins**: Shows how to add standard platform views to the map.
- **Routing**: Shows how to calculate routes and add them to the map.
- **Navigation**: Shows turn-by-turn navigation and tracking. Exclusively available for the _Navigate Edition_.
- **Search**: Shows how to search POIs and add them to the map.
- **Traffic**: Shows how to search for real-time traffic and how to visualize it on the map.
- **StandAloneEngine**: Shows how to use an engine without a map view.

Most example apps contain a class named "XY-Example" where XY stands for the feature, which is in most cases equal to the name of the app. If you are looking for example code that shows how to use a certain HERE SDK feature, then please look for this class as it contains the most interesting parts. Note that the overall app architecture is kept as simple as possible to not shadow the parts in focus.

> Not all examples are available for all editions and platforms.

Find the examples for the edition and platform of your choice:

- HERE SDK for Android ([Lite Edition](examples/latest/lite/android/), [Explore Edition](examples/latest/explore/android/), [Navigate Edition](examples/latest/navigate/android/))
- HERE SDK for iOS ([Lite Edition](examples/latest/lite/ios/), [Explore Edition](examples/latest/explore/ios/), [Navigate Edition](examples/latest/navigate/ios/))
- HERE SDK for Flutter ([Explore Edition](examples/latest/explore/flutter/), [Navigate Edition](examples/latest/navigate/flutter/))

## Example Apps for Other Versions
In addition to the apps above, this repo also contains example apps for the following HERE SDK versions:
- [Version 4.3.4.0](examples/4.3.4.0/)
- [Version 4.3.3.0](examples/4.3.3.0/)
- [Version 4.3.2.0](examples/4.3.2.0/)
- [Version 4.3.1.0](examples/4.3.1.0/)
- [Version 4.3.0.0](examples/4.3.0.0/)
- [Version 4.2.1.0](examples/4.2.1.0/)
- [Version 4.2.0.0](examples/4.2.0.0/)

## What You Need to Execute the Example Apps
1. Acquire a set of credentials by registering yourself on [developer.here.com](https://developer.here.com/) - or ask your HERE representative.
2. Download the latest HERE SDK artifacts for your desired platform. These can be found on [developer.here.com](https://developer.here.com/) unless otherwise noted.
3. Please refer to the minimum requirements and supported devices as listed in our _Developer's Guide_.

### Get Started for Android
1. Copy the AAR file of the HERE SDK for Android to the example app's `app/libs` folder.
2. Open _Android Studio_ and sync the project.
3. To run the app, you need to add your HERE SDK credentials to the `AndroidManifext.xml` file.

### Get Started for iOS
1. Copy the `heresdk.framework` file of the HERE SDK for iOS to the example app's root folder.
2. In Xcode, open the _General_ settings of the app target and make sure that the HERE SDK framework appears under _Embedded Binaries_. If it does not appear, add the `heresdk.framework` to the _Embedded Binaries_ section ("Add other..." -> "Create folder references").
3. To run the app, you need to add your HERE SDK credentials to the `Info.plist` file.

### Get Started for Flutter
1. Unzip the HERE SDK for Flutter plugin to the `plugins` folder that can be found inside the example app project. Renname the folder to 'here_sdk': hello_map/plugins/here_sdk
2. Set your HERE SDK credentials to
  - `hello_map/android/app/src/main/AndroidManifest.xml`
  - `hello_map/ios/Runner/Info.plist`
3. Start an Android emulator or an iOS simulator and execute `flutter run` from the app's directory - or run the app from within your IDE.

## Get in Touch
If you have more questions, please check [stackoverflow.com/questions/tagged/here-api](http://stackoverflow.com/questions/tagged/here-api). Information on how to contribute to this project can be found [here](CONTRIBUTING.md). If you have questions about billing or your account, [contact us](https://developer.here.com/contact-us). Thank you for using the HERE SDK.

## License
Copyright (C) 2019-2020 HERE Europe B.V.

See the [LICENSE](LICENSE) file in the root of this repository for license details.
