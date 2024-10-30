# neXtgen 🌍📱

## [Contributors guide 🔗](https://github.com/Vishwajith-Shettigar/NextGen/blob/develop/CONTRIBUTORS.md)



## Overview 🌟
Interact with people within a 100-meter radius! Get real-time locations of nearby folks on Google Maps and chat or have a video call with them. If the conversation wasn’t up to par, you can give them a solid 0-star rating. 😄👎

## Features 🚀
- **Real-time Location:** Spy on the real-time whereabouts of nearby users on Google Maps. 🕵️‍♂️🗺️
- **Chat:** Send some text magic to nearby users. 💬🧙‍♂️
- **Video Call:** Face-to-face chats with nearby users using the power of WebRTC. 📹👥
- **Rating System:** Rate your chat experience. If it was a dud, slap them with a 0-star review. 🌟😢

## Technologies Used 🛠️
- **Android:** The app is tailor-made for Android devices. 🤖📱
- **Firebase:** Powering up authentication, real-time database awesomeness, and storage ninja skills. 🔥🧙‍♀️
- **WebRTC:** Real-time video calling sorcery. Let the calls flow like magic! 🎩🔮
- **Google Maps API:** Pinpointing the exact coordinates of your newfound friends. 📍🗺️
- **Kotlin:** The language of choice for Android wizardry. It’s like casting spells with code! 🧙‍♂️✨

## Screenshots 📸

<table>
  <tr>
    <td><img src="https://avatars.githubusercontent.com/u/176493940?v=4" width="100px"alt="Zafar Ali""/></td>
    <p><a href="https://github.com/zafar-Alee" target="_blank"> Zafar Ali</a></p>
  </p>
</table>

---

Time to mingle, chat, and rate! Have fun exploring the world around you. 🌍🎉

## Troubleshooting 🤔
If you encounter any issues while setting up or using NextGen, try the following troubleshooting tips.

### 1. Build Fails with Gradle Errors
- **Issue:** Errors related to Gradle during the build process.
- **Solution:** Ensure you have the correct version of Gradle and Android Studio installed. Check the `build.gradle` files to verify dependencies are compatible.

**Additional Tip from #75:**
- **Issue:** Incompatible Java version settings causing errors such as `kaptGenerateStubsDebugKotlin` task failures.
- **Solution:** Make sure `JAVA_HOME` is set to JDK 17 in the environment variables. In the `build.gradle` files, specify:
  ```gradle
  android {
      compileOptions {
          sourceCompatibility JavaVersion.VERSION_1_8
          targetCompatibility JavaVersion.VERSION_1_8
      }
      kotlinOptions {
          jvmTarget = "1.8"
      }
  }
  ```

### 2. Missing SDK Components
- **Issue:** Build failure due to missing SDK components.
- **Solution:** Check for required packages using the SDK Manager in Android Studio and install any missing dependencies.

### 3. Dependency Conflicts
- **Issue:** Conflicts between libraries or dependencies causing build issues.
- **Solution:** Review the `build.gradle` files and check for any version conflicts. Updating the library versions to be compatible might solve the issue.

### 4. Insufficient Memory During Build
- **Issue:** Running out of memory while building the project.
- **Solution:** Increase the heap size in the `gradle.properties` file. Try allocating more memory to the Gradle build by updating:
  ```properties
  org.gradle.jvmargs=-Xmx2048m
  ```

### 5. Clarification on SERVER_URL in secrets.properties from #47
**Issue:** Uncertainty about the value to use for SERVER_URL.
**Solution:** If you are not working on the video call feature, please add any random characters as a workaround (e.g., SERVER_URL=pbdwkw). This variable holds the video call server URL. 
You can find the repository for reference [here](https://github.com/Vishwajith-Shettigar/video-call-server-node.js).

## TODO 📝
- [ ] Enhance UX of video call feature.
- [ ] Notification UI.
- [ ] Improve UI/UX.
- [ ] Fix crashing when user swtiches to light/dark mode.

