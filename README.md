# Template
This is a starting maven template for [RenJava](https://github.com/HackusatePvP/RenJava). Download the code and extract to projects folder. Open with an IDEA of your choosing and follow the instructions to build the project.

## IDEA
I personally use [intellij](https://www.jetbrains.com/idea/). If you are using RenJava for commercial use please read the license.
Some IDEA require you to purchase a license for commercial use. This is not legal advice.

## Make sure...
Make sure you change the pom.xml information. Below is an example of what you can change it to.
```xml
<groupId>me.youridentifier</groupId>
<artifactId>yourgame</artifactId>
<version>1.0.0</version>
```

Verify the pom is using the latest version of RenJava.
```xml
<dependency>
  <groupId>me.piitex</groupId>
  <artifactId>RenJava</artifactId>
  <version>change to latest version</version>
</dependency>
```
Change the packaging scheme to match the artifact and group id. This is important as the build folder will look weird if you don't.

## Important
Please download and run [RSDK](https://github.com/HackusatePvP/RenJavaSDK/releases). Follow the instructions RSDK provides. Change the groupid and artifact before running RSDK.

## Building and Testing
Use `mvn clean install` to compile the project. Use RSDK to create the testing environment. Use the 'start.bat' to test your game as you make it.

Note: You will have to re-compile everytime you modify the code. `mvn clean install`. Put that newly built jar file which is located in `target/` inside the testing directory. Overwrite the file if prompted.