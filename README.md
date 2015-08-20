# Maven

There are three things about Maven that are very nice.


1.Maven will (after you declare which ones you are using) download all the libraries that you use and and the libraries that they they use for you automatically. This is very nice, and makes dealing with lots of libraries ridiculously easy. This lets you avoid "depenendency hell". It is similar to Apache Ant's Ivy.

2.It uses "Convention over Configuration" so that by default you don't need to define the tasks you want to do. You don't need to write a "compile", "test", "package", or "clean" step like you would have to in Ant or a Makefile. Just put the files in the places Maven expects them and it should work off of the bat.

3.Maven also has lots of nice plug-ins that you can install that will handle many routine tasks from generating Java classes from an XSD schema using JAXB to measuring test coverage with Cobertura. Just add them to your pom.xml and they will integrate with everything else you want to do.


What is Maven Repository? 

Maven仓库就是放置所有JAR文件（WAR，ZIP，POM等等）的地方，所有Maven项目可以从同一个Maven仓库中获取自己所需要的依赖JAR，这节省了磁盘资源。此外，由于Maven仓库中所有的JAR都有其自己的坐标，该坐标告诉Maven它的组ID，构件ID，版本，打包方式等等，因此Maven项目可以方便的进行依赖版本管理。你也不在需要提交JAR文件到SCM仓库中，你可以建立一个组织层次的Maven仓库，供所有成员使用。



Usally used command in Maven:

1. mvn -v : check the version of Maven

2. mvn compile : to compile

3. mvn package: take the compiled code and package it in its distributable format, such as a JAR.

4. mvn clean: delete the targe file;attempts to clean a project's working directory of the files that we're generated at build-time

5. mvn install: 在本地Repository中安装jar； install jar files in the local Repository.


