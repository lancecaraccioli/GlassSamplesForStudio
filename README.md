GlassSamplesForStudio
=====================

The standard Google Glass Samples ported into an Android Studio 0.4.3 project.

Assumptions
-----------

* The basic infrastructure is prepared
  * Android Studio is installed and up to date (Currently version 0.4.3)
  * The necessary SDKs are installed
    * Java SDK
    * Android 4.0.3
    * Glass Development Kit Sneak Peek

Tested Environment State
------------------------

* Ubuntu 14.04
  * Oracle Java 7 JDK
  * Android Studio 0.4.3
    * Android 4.0.3 (API 15)
      * SDK Platform
      * Glass Development Kit Sneak Peek
    * Gradle 1.10

Tips
----

* When creating a new module...
  * Minimum required SDK: API 15...
  * Target SDK: API 15...
  * Compile with: Glass Development Kit Sneak Peak...
  * (The relevant bit) After creating the module you will still need to update one line in your modules build.gradle file
    * - compileSdkVersion 15
    * + compileSdkVersion "Google Inc.:Glass Development Kit Sneak Peek:15"
  * See [http://stackoverflow.com/questions/20107002/google-glass-gdk-with-android-studio]

* When running a module for the first time...
  * On the "General" tab; under the "Activity" group
    * Select "Launch"
    * Chose the menu activity associated with that Sample.
      * compass: com.google.android.glass.sample.compass.CompassMenuActivity
      * stopwatch: com.google.android.glass.sample.stopwatch.MenuActivity
      * timer: com.google.android.glass.sample.timer.MenuActivity

