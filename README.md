# KMP Onsite Demo
In this activity, you will create an app that uses both Kotlin Multiplatform and Compose Multiplatform. You will:
* Use Kotlin Multiplatform's expect/actual framework to write platform-specific code for both the iOS and Android apps
* Use Compose Multiplatform to create a shared UI view


## Setup:
1.  Download the [latest version of Android Studio](https://developer.android.com/studio?gad_source=1&gclid=Cj0KCQjw_-GxBhC1ARIsADGgDjsUCtp_3alj-xGYQR4-upl9qy0uo4SFEg3fFH3mlvFRQTx_YtaMx1QaAmPuEALw_wcB&gclsrc=aw.ds)
2.  Clone this project locally:
    `git clone git@github.com:upside-sarah/kmp-onsite-demo.git`
3. Open the project in Android Studio

## Activity:
Now, write a platform-specific function and call it from your common code!

1. Locate the `commonMain` folder, where the shared code is written. Write your `expect` function signature in `YourExpectFun.kt`
2. Implement the `actual` functions in each platform-specific module. Feel free to access platform-specific APIs here!
3. Call your `expect` function from the shared code in `App`
4. Hit the play button to run the Android app!

## Bonus (time permitting):
To run the app on iOS, install the KMM plugin:
1. `Android Studio` -> `Settings` -> `Plugins` -> `Marketplace` -> `Kotlin Multiplatform Mobile`
2. Install the plugin and restart Android Studio
3. Next to the run button, click the dropdown and select `iosApp`
4. Click the run button to run the iOS app!


# ! Cheat codes: Only read below if you're stuck !
* Tip: `CMD + Shift + F` to find all of the `TODO`s and fill in your code
* In `YourExpectFun.kt`, write a simple function signature (`fun someMethod(): String`)
* The IDE should warn that your platform targets don't have `actual` declarations for your function.
  * Hover over the error and click "Add missing actual declarations" to auto-generate the methods
* In `App.kt`, create a `TextView` composable that displays your string