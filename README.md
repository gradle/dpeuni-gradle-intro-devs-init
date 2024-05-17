# DPE University Training

<p align="left">
<img width="10%" height="10%" src="https://user-images.githubusercontent.com/120980/174325546-8558160b-7f16-42cb-af0f-511849f22ebc.png">
</p>

## Gradle Init Exercise

This is a hands-on exercise to go along with the
[Introduction to Gradle Build Tool for Developers](https://dpeuniversity.gradle.com/app/courses/012de84f-fcd3-45d4-9c4c-284382eb3f3f)
training module. In this exercise you will go over the following:

* Initializing new Gradle project
* Opening a Gradle project in an editor
* Explore Gradle files

---
## Prerequisites

* JDK 1.8+ and a recent version of Gradle build tool installed
    * https://gradle.org/install/
* A good editor such as IntelliJ IDE
    * https://www.jetbrains.com/idea/download/

---
## Initialize new Gradle Project

1. Open a terminal and create a folder called `lab`, then go inside it. Initialize a new Gradle
   project by running the `gradle init` command and enter the following responses
   for the questions:

**Note**: The questions `gradle init` asks may differ for different version of Gradle build tool.

* Type of build to generate: application
* Language: Java
* Java version: Execute `java -version` to find version
* Project name: lab
* Application structure: single application
* Build script DSL: Kotlin
* Test framework: JUnit Jupiter
* Use new APIs?: no

```
$ gradle init

Select type of build to generate:
  1: Application
  2: Library
  3: Gradle plugin
  4: Basic (build structure only)
Enter selection (default: Application) [1..4] 

Select implementation language:
  1: Java
  2: Kotlin
  3: Groovy
  4: Scala
  5: C++
  6: Swift
Enter selection (default: Java) [1..6] 

Enter target Java version (min: 7, default: 21): 11

Project name (default: lab):

Select application structure:
  1: Single application project
  2: Application and library project
Enter selection (default: Single application project) [1..2] 

Select build script DSL:
  1: Kotlin
  2: Groovy
Enter selection (default: Kotlin) [1..2] 

Select test framework:
  1: JUnit 4
  2: TestNG
  3: Spock
  4: JUnit Jupiter
Enter selection (default: JUnit Jupiter) [1..4] 

Generate build using new APIs and behavior (some features may change in the next minor release)? (default: no) [yes, no] 
```

2. Ensure the generated files in the solution directory look as follows:

```
$ ls -ltr
total 32
drwxr-xr-x  3 adayal  staff    96 May 12 06:35 gradle
-rwxr-xr-x  1 adayal  staff  8070 May 12 06:35 gradlew
-rw-r--r--  1 adayal  staff  2763 May 12 06:35 gradlew.bat
-rw-r--r--  1 adayal  staff   372 May 12 06:38 settings.gradle.kts
drwxr-xr-x  4 adayal  staff   128 May 12 06:38 app
```

---
## Open Project in Editor and Explore Files

1. Launch your Editor and open the `lab` folder

2. Look at the following files:

* `settings.gradle.kts`
* `app/build.gradle.kts`
* `gradle/wrapper/gradle-wrapper.properties`

3. In the `app/build.gradle.kts` file hover over the `mavenCentral()` word and
   notice the help tooltip popup.

<p align="center">
<img width="60%" height="60%" src="https://user-images.githubusercontent.com/120980/174327421-da264871-bad8-4d36-bd23-e156eeeebbcb.png">
</p>

4. Notice sample sources and tests have been created:

* `app/src/main/java/com/gradle/lab/App.java`
* `app/src/test/java/com/gradle/lab/AppTest.java`

<p align="center">
<img width="60%" height="60%" src="https://user-images.githubusercontent.com/120980/174327548-d03ad27f-32c7-4e44-a111-04de4cc21fa3.png">
</p>