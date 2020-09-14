### This is a fork of [OneSignal-Android-SDK](https://github.com/OneSignal/OneSignal-Android-SDK)

that allows you to specify a custom base url in case you need to use a proxy server...

This fork is based in the source code of version:
![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.onesignal/OneSignal/badge.svg)

----

### How to use
You just need to set the **baseUrl** in the OneSignal.init(...) function like:

```
OneSignal.init(
         this,
         "1234567", // This is ignored, dashboard value will be used.
         "aaaaa-aaaaa-aaaaa-aaaaa", //your app-id
         "https://my.domain.com", //your custom baseUrl  
         new ExampleNotificationOpenedHandler(),
         new ExampleNotificationReceivedHandler()
      );
```