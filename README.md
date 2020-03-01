# UnityAndroidToasty

Sample to solve Android dependent library by gradle.

- Unity Project: [UnityAndroidToasty](UnityAndroidToasty)
- Android Project: [ToastyWrapper](ToastyWrapper)

## Requirements

- Unity2019.3.9f1
    - Android Build Support Module
- Android Studio 3.6.2

## How to build

1. copy `classes.jar` in Unity Editor to `ToastyWrapper/toastywrapper/libs/`  
see also https://docs.unity3d.com/Manual/AndroidUnityPlayerActivity.html
1. build android library

        $ cd ToastyWrapper
        $ ./gradlew clean build
1. publish android library to [m2repository](UnityAndroidToasty/Assets/m2repository/)

        $ ./gradlew publish
1. build app with unity
