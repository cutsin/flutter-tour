# Develop Environments

## ENV

```Shell
FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
PUB_HOSTED_URL=https://pub.flutter-io.cn
```

## Android Studio

* Proxy: Configure -> Settings -> System Settings -> HTTP Proxy, Check `Auto-detect proxy settings` & `Automatic proxy configuration URL`: `mirrors.neusoft.edu.cn:80`

## VSCode

* Disable `Allow Analytics` for Dart process high CPU load
* Disable `search.followSymlinks` for high cpu load
* Proxy (Socks 5)

 * Open `~/.gradle/gradle.properties`

   ```
   org.gradle.jvmargs=-DsocksProxyHost=127.0.0.1 -DsocksProxyPort=1081
   ```
