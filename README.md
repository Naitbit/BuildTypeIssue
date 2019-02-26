# BuildTypeIssue
Example of AndroidStudio green arrow run method issue in instrumented tests

After `testBuildType` is set in `build.gradle` the "green arrow" in Android Studio is no longer working.
Instead of expected behaviour of creating "Android Instrumented Tests" configuration
it creates "Android JUnit" configurations instead:
![Method configuration - incorrect](static/Method_arrow_failure.png)
Running "Android JUnit" fails with no tests found.

Using run on whole class does create correct configuration which works:
![Class configuration - correct](static/Class_arrow_working.png)
