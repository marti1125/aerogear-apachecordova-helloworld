Create an app with Apache Cordova 3.4.0
=======================================

###Setup Apache Cordova in Windows

**Prerequisites**

* Node.js
* Apache Ant
* Android ADT Bundle for windows

**Setup Node.js**

Download and install node.js from [Nodejs Download](http://nodejs.org/download/) and verify the installation by typing the following command in the command prompt.

![nodev](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/nodev.png)

**Setup Apache Ant**

Before downloading Ant make sure that JDK is already installed in your computer. If not download the JDK ([JDK Download](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)) and install it before setting Ant. 

Download apache-ant-x.x.x-bin.zip from [Ant Download](http://ant.apache.org/bindownload.cgi) and extract the contents to a directory (Eg., E:\Tools\Project\Build\apache-ant-x.x.x). This directory will be known as ANT_HOME.

Open environment variables (Control Panel » System » Advanced » Environment Variables) add a new system variable as displayed below, 

![anthome](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/ant_home.png)

Set the %ANT_HOME%\bin; to the path as displayed below,

![antpath](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/Ant_Path.png)

Verify the installation of Ant by typing the following command in the command prompt, 

![antv](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/apacheantv.png)

If you get any other messages related to java, then you need to check if JAVA_HOME is available in the environment variables. Else make sure to add the JDK installation path to the system variable and add %JAVA_HOME%\bin; to the path variable.

It is important to note that whenever the environment variables are modified, a new command prompt should be opened to verify the installation.

**Setup Android ADT Bundle for Windows**

As this article speaks about installing cordova for developing the apps for the android platform, it is important to download the [Android Developer Tools](http://developer.android.com/sdk/index.html) and make sure that it is available in the system classpath.

If you are developing apps for other platforms, make sure that the developer tools or sdk for the platform is available in your classpath.

Extract the downloaded adt-bundle-windows-xxx_xx-xxxxxxxx.zip to a directory (E:\Tools\Project\android\adt-bundle-windows-x86_64-20130729). 

This directory will contain the sdk for android. Add tools and platform-tools to the path variable of the environment variables as displayed below,

![androidsdktools](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/platform_tools_path.png)

Once the environment is setup, an Android Virtual Device (AVD) should be added. The Virtual device is the target device on which the application created using cordova will be tested. The best resource for creating an AVD is [Managing AVD](http://developer.android.com/tools/devices/managing-avds.html)

**Hurrah All Set**


All the required dependencies for setting up cordova has been already installed. Now lets get started with installing cordova using nodejs.

Open the command prompt and type the command,

    npm install -g cordova

This command will download the latest version of all the node modules required by cordova. 

Verify the installation of Cordova by typing the following command in the command prompt,

![cordovav](https://raw.github.com/marti1125/aerogear-apachecordova-helloworld/master/doc/cordovav.png)

