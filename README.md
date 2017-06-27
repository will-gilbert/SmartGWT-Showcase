# SmartGWT-Showcase
## A Gradle build for Isomorphics' SmartGWT LPGL Showcase

*https://github.com/will-gilbert/SmartGWT-Showcase*

You need to download two Jar files, ```smartgwt-skins.jar``` and ```smartgwt.jar``` into the ```lib/SmartGWT-X.X-LPGL``` directory of this project, where ```X.X``` is the version number of the release, *e.g.* 6.1 as shown below.

![Library Layout](Layout.png)

These LGPL licensed SmartGWT library files can be downloaded from the **Isomophics.com** website at :

*http://www.smartclient.com/product/download.jsp*

The target browser(s) can be set using the ```gradle.properties``` file by setting the comma delimited ```user.agent``` property.


```
#  Build for the following browsers:
#
#     safari : Apple Safari, Google Chrome, WebKit broswers
#   gecko1_8 : FireFox
#        ie6 : Windows IE6 and IE7
#        ie8 : Windows IE8
#        ie9 : Windows IE9
#      opera : Opera
#     iphone : iPhone
#

user.agent=safari,gecko1_8

```

Gradle wrapper has been provided which uses Gradle v3.5. Use the Gradle task ```./gradlew usage``` to build and run the Showcase.


If you choose to install and use Gradle, note that this build uses the Gradle ```jetty``` plugin which is deprecated in Gradle 4.0.  Use Gradle v3.5 until the build is rewritten to use the new ```gretty``` plugin.

