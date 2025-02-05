[![official JetBrains project](http://jb.gg/badges/official-plastic.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)

Kotlin Koans(Kotlin语法---官方系列教程)
===========

Kotlin Koans Workshop is a series of exercises to get you familiar with the Kotlin Syntax. 
Each exercise is created as a failing unit test and your job is to make it pass. 

#### How to build and run tests

##### Working with the project using Intellij IDEA or Android Studio:

1. Import the project as Gradle project.
2. To build the project and run tests use `test` task on Gradle panel. 

Here https://www.jetbrains.com/help/idea/gradle.html you can read how to work with Gradle projects in IntelliJ IDEA.

##### Working with the commandline

You can also build the project and run all tests in the terminal:
```
./gradlew test
```
But since running all the tests tend to take longer and the output can be
cluttered, it's more ideal to run selected tests only:
```
$ ./gradlew test --tests i_*          # run tests in part 1
$ ./gradlew test --tests ii_*         # run tests in part 2
$ ./gradlew test --tests ii_*22*      # run test number 22 in part 2
```


#### How to check yourself

The repository has two branches, `master` which contains the exercises for you to do and `resolutions` which contains the resolved exercises. 
Make sure you don’t cheat!


#### How the tasks are organized
 
You have 42 tasks to do. 
Each task lives in its own function: from `task0` to `task41`.
For each task, there is an associated unit test that checks your solution.
 
You may navigate to the corresponding test automatically when you read the task.
Open the source file with the task and use the action `Navigate -> Test` to open the test file. 
You may also use `Navigate -> Test Subject` for reversed navigation.

Individual tasks generally require you to change the function `taskX` by completely replacing the body of the function.
Your goal is to solve the problem and allow the associated unit test to pass. 
If you run the unit test for a task that is not correct, the unit test results will be displayed. 
If you have not yet made any changes to a task, the exception will be thrown and the task's TODO message will be displayed. 

In the first example, this means replacing the code

```kotlin
fun task0(): String {
    return todoTask0()
}
```

with the correct, meaningful code in order to solve the problem and allow the associated unit test to pass, such as:

```kotlin
fun task0() = "OK"
```

The `resolutions` branch contains all the solutions.
It's a good idea to check the proposed solution after completing each task.
Open the file with your solution, call the `Compare with branch...` action and choose the `resolutions` branch.   
You can find [here](https://www.jetbrains.com/help/idea/navigating-to-action.html) how to call an action.


#### Other ways to solve Koans

You can solve the similar tasks using Educational Plugin or in the browser:

- Educational Plugin https://blog.jetbrains.com/kotlin/2016/03/kotlin-educational-plugin
- online version of koans http://try.kotl.in

The koans tasks for web-demo and educational plugin can be found here: https://github.com/Kotlin/kotlin-koans-edu
