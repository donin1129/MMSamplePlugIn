# About this project

This project is meant to serve as an example how to write plugin for micro-manager-2.0 using Gradle Kotlin build system in a mordern IDE such as IntelliJ. 


## How to work with this? 

### 1. Install Micro-Manager 2.0
Install Micro-Manager 2.0 from https://micro-manager.org/Download_Micro-Manager_Latest_Release. 

### 2. Install JDK
You can use suggested JDK from as suggested your system to work with JDK 2.0 from https://micro-manager.org/Writing_plugins_for_Micro-Manager#setting-up-to-write-debug-and-package-plugins.

You can also install your JDK of your choice to see if it works. 

### 3. Build jar

Use command ```.\gradlew build```
Or use IDE convenient tools to build jar. 

### 4. Copy jar from build location to mmplugins directory

After the build, a file will be generated at `./build/libs/MMPlugInSample-1.0.jar`. 
Copy this file and add it to mmplugins directory. In Windows, it should be located at `C:\Program Files\Micro-Manager-2.0\mmplugins`. 

### 5. Start Micro-Manager 2.0

You should be able to find the plugin at `Plugins | Developer Tools | Hello, World! ` once you configure Micro-Manager. 

The location of the plugin is defined by your code at `./src/main/java/com/example/helloworld/HelloWorldPlugin.java`. See comments there. 

You can find more examples at https://github.com/micro-manager/micro-manager/tree/main/plugins. The code in this example project is from https://github.com/micro-manager/micro-manager/tree/main/plugins/HelloWorld. 

## System Considerations

* I have **Windows 10 Pro** but any Windows system should work with this project. (Not sure how it will behave on a Unix)
* I am using JDK temurin-1.8 from https://adoptium.net/temurin/releases/?version=8&package=jdk&arch=x64&os=windows as suggested here https://micro-manager.org/Writing_plugins_for_Micro-Manager. But other JDK might work as well. 
