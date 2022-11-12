# lockscreenwidget

## About lockscreenwidget
Testing purpose

## Environment Setup
+ OS- macOS Monterey(version - 12.6)
+ Android Studio version - Chipmunk | 2021.2.1
+ Android SDK version - 32

## Installing the Android SDK
Once installed, open Android Studio. The IDE should detect that the Android SDK needs to be installed.
In the SDK Components Setup screen, finish installing the SDK. Keep note of the Android SDK Location.
By default, the latest stable SDK Platform is installed, which includes a collection of packages required to target that version of Android.

## Configuring Command Line Tools
+ Some environment variables must be set. The following instructions are for macOS
+ In ~/.bashrc, ~/.bash_profile, or similar shell startup scripts, make the following modifications:
    1. Set the ANDROID_SDK_ROOT environment variable. This path should be the Android SDK Location used in the previous section.
        $ export ANDROID_SDK_ROOT=$HOME/Android/sdk
    2. Add the Android SDK command-line directories to PATH. Each directory corresponds to the category of command-line tool.
     - $ # avdmanager, sdkmanager
     - $ export PATH=$PATH:$ANDROID_SDK_ROOT/tools/bin
     - $ # adb, logcat
     - $ export PATH=$PATH:$ANDROID_SDK_ROOT/platform-tools
     - $ # emulator
     - $ export PATH=$PATH:$ANDROID_SDK_ROOT/emulator


## Folder Structure
+ Here is the core folder structure of lockscreenwidget app.
+ lockscreenwidget/
- app
    - src
        - main
            - java files
            - xml files
            - manifest.xml
    - build.gradle
- gradle
