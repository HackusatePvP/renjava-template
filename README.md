# Template
This is a starting maven template for [RenJava](https://github.com/HackusatePvP/RenJava). Download the code and extract to projects folder. Open with an IDEA of your choosing and follow the instructions to build the project.

## IDEA
The following are links to IDEA's (integrated development environment application) you can use.
- [Intellij](https://www.jetbrains.com/idea/) (See license for information about commercial use)
- [Visual Studio Code](https://code.visualstudio.com) (Free for private and commercial use. See license for more information.)
- [Eclipse](https://www.eclipse.org/downloads/) (See license for information about commercial use)

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
Change the packaging scheme to match the artifact and group id. Rename the directories 'template' and `renjava` to `groupid`. An example would be changing `template/renjava` to `me/piitex`.

## Important
Please download and run [RSDK](https://github.com/HackusatePvP/RenJavaSDK/releases). Follow the instructions RSDK provides. Change the groupid and artifact before running RSDK.

In a terminal/command prompt at the main directory of the project run `java -jar {placeholder}.jar -- color {color}` Where {placeholder} is the RSDK jar file name and {color} is the default color scheme you want.
RSDK lists all supported colors in the README.md file.

## Building and Testing
Use `mvn clean install` to compile the project. Use RSDK to create the testing environment. Use the 'start.bat' to test your game as you make it.

Note: You will have to re-compile everytime you modify the code. `mvn clean install`. Put that newly built jar file which is located in `target/` inside the testing/environment directory. Overwrite the file if prompted.