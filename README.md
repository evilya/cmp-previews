This is a Kotlin Multiplatform project targeting Android, iOS, Desktop (JVM).

* [/shared](./shared/src) contains shared code used by all entry points.
  It contains several subfolders:
  - [commonMain](./shared/src/commonMain/kotlin) is for code that is common for all targets.
  - [androidMain](./shared/src/androidMain/kotlin), [iosMain](./shared/src/iosMain/kotlin), and [jvmMain](./shared/src/jvmMain/kotlin)
    are for platform-specific shared implementations.

* [/androidApp](./androidApp/src/main) contains the Android application entry point.
* [/desktopApp](./desktopApp/src/jvmMain) contains the Desktop (JVM) application entry point.
* [/iosApp](./iosApp/iosApp) contains the iOS application wrapper and SwiftUI entry point.

### Build and Run Android Application

To build and run the development version of the Android app, use the run configuration from the run widget
in your IDE’s toolbar or build it directly from the terminal:
- on macOS/Linux
  ```shell
  ./gradlew :androidApp:assembleDebug
  ```
- on Windows
  ```shell
  .\gradlew.bat :androidApp:assembleDebug
  ```

### Build and Run Desktop (JVM) Application

To build and run the development version of the desktop app, use the run configuration from the run widget
in your IDE’s toolbar or run it directly from the terminal:
- on macOS/Linux
  ```shell
  ./gradlew :desktopApp:run
  ```
- on Windows
  ```shell
  .\gradlew.bat :desktopApp:run
  ```

### Build and Run iOS Application

To build and run the development version of the iOS app, use the run configuration from the run widget
in your IDE’s toolbar or open the [/iosApp](./iosApp) directory in Xcode and run it from there.

---

Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)…
