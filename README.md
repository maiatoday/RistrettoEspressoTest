# RistrettoEspressoTest

Basic Espresso Hello World

Clone the project, import the project into Android Studio by choosing the build.gradle file.

To run the unit tests from the command line run `./gradlew test`

To run the functional tests from the command line, open an emulator of your choice and run `./gradlew cC`

To setup a run configuration in Android studio for either set of tests edit the configurations in the following way:

Unit tests:
![Unit test run configuration](ScreenshotUnitTest.png)

Funtional tests with espresso:
![Functional test run configruation](ScreenshotFunctionalTest.png)

When you switch between the two sets of tests also remember to switch Test artifact in the Build Variants tab in Android studio.


![Build variants](buildVariants.png)

## Making it build

* Copy the signing.properties.template file to signing.properties
* Put debug.keystore file from ~/.android into app directory
* If you want to build a release version, make a keystore file and put it in the app directory with the name release-key.keystore or change the name in the signing.properties file. Also fill in the alias and password in the signing.properties file.
* Make sure the release-key.keystore or it's equivalent is in the .gitignore in the app directory so that you don't check it into the project.
