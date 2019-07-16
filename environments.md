# Develop Environments

## Host (Windows)

```Shell
set FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
set PUB_HOSTED_URL=https://pub.flutter-io.cn
```

# VSCode

* Disable `Allow Analytics` for Dart process high CPU load
* Disable `search.followSymlinks` for high cpu load
* Mirrors:
  * Open `your_flutter_source_root/packages/flutter_tools/gradle/flutter.gradle`:
    
    ```
    repositories {
      // google()
      // jcenter()
      maven { url 'https://maven.aliyun.com/repository/google' }
      maven { url 'https://maven.aliyun.com/repository/jcenter' }
      maven { url 'http://maven.aliyun.com/nexus/content/groups/public' }
    }
    ```
  * Open `your_project_path/android/build.gradle`:
    
    ```
    repositories {
      // google()
      // jcenter()
      maven { url 'https://maven.aliyun.com/repository/google' }
      maven { url 'https://maven.aliyun.com/repository/jcenter' }
      maven { url 'http://maven.aliyun.com/nexus/content/groups/public' }
    }
