# Kotlin Desktop GUI Template
### Project Template to build a Desktop App with the Compose Framework
### using Gradle (i.e. without an IDE)

Create a project template so that a Desktop GUI can be coded, with the aid of Compose Framework, without the use of IntelliJ or Android Studio, which are heavy on memory consumption. This is even more useful on older machines. 

Just code your application with an editor/text editor of your choice (mousepad, vim, emacs etc..), and compile/run the project by running:

``` gradle run ```

Using Gradle has lots of requirements, and errors might still pop up due to having installed things incorrectly. It is a careful time-consuming process, requires attention to detail and OS knowledge (settings environment variables etc...), as things will not work 'out of the box.'

### Requirements:

Java SDK:

``` apt-get install default-jdk ```

Android SDK:

``` apt-get install android-sdk ```

Update environment variables:

```mousepad ~/.bashrc```

at the bottom:

``` export ANDROID_SDK_ROOT=/usr/share/android-sdk/ (The path of your android installation)```

Latest Gradle version (https://github.com/gradle/gradle/releases/), manually installed or install with sdkman.

Finally, change 'group = "me.user"' in the file 'build.gradle.kts' to your own name:

``` sed -i 's/me.user/me.myname/g' build.gradle.kts ```

Update android SDK with the aid of sdk package manager:

``` android update sdk ```

if "Failed to create /<PATH>/build-tools - platforms - add-ons":

``` mkdir build-tools platforms add-ons ```

Missing platform-tools? Install them!
 

