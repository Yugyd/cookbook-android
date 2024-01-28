Cookbook Android
================

Cookbook Android is a Open Source knowledge testing platform for Android based on Jetpack Compose and
Google solutions. The project is based on the latest Android development solutions and can act as a
sample for other developers.

Coming soon app "Cookbook Android" on Google Play.

# Stack

The project is developed strictly within the framework of the Google way, only Google solutions are
used. For novice developers to dive into android development.

* Language: Kotlin
* Architecture: MVVM (Google), clean, multi-module
* UI: Compose, Material 3
* Navigation: Jetpack Compose Navigation
* Threading: Coroutines + Flow
* DI: Hilt
* DB: Room
* Image: Coil
* Mobile services: Firebase
* Logging: Timber
* Testing: JUnit4, Mockk

# Build types

The debug build option can be built and run. The release option is used on internal projects and
is not publicly available, you need a real Firebase project to access it.

Debug - Logging, debug mode, proguard off.

Release - No logging, no debug mode, proguard enabled.

# Deploy to Firebase App Distribution

Use environment variable `FIREBASE_APP_ID`. Set your app id value from Firebase.

https://docs.gradle.org/current/userguide/build_environment.html#sec:gradle_environment_variables

# Contributions

[Guide](docs/CONTRIBUTION.md)

# Build

## Deploy debug to Firebase App Distribution

- `./gradlew clean bundleDebug`
- `./gradlew appDistributionUploadDebug`

## Deploy release to Firebase App Distribution

- `./gradlew clean bundleRelease`
- `./gradlew appDistributionUploadRelease`

## Upload to Google Play

- `./gradlew clean bundleRelease`
- Manual upload to Google Play

# License

```
   Copyright 2024 Roman Likhachev

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
