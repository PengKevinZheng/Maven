# Maven

There are three things about Maven that are very nice.


1.Maven will (after you declare which ones you are using) download all the libraries that you use and and the libraries that they they use for you automatically. This is very nice, and makes dealing with lots of libraries ridiculously easy. This lets you avoid "depenendency hell". It is similar to Apache Ant's Ivy.

2.It uses "Convention over Configuration" so that by default you don't need to define the tasks you want to do. You don't need to write a "compile", "test", "package", or "clean" step like you would have to in Ant or a Makefile. Just put the files in the places Maven expects them and it should work off of the bat.

3.Maven also has lots of nice plug-ins that you can install that will handle many routine tasks from generating Java classes from an XSD schema using JAXB to measuring test coverage with Cobertura. Just add them to your pom.xml and they will integrate with everything else you want to do.


Usally used command in Maven:

1. mvn -v : check the version of Maven

2. mvn compile : to compile

3. mvn package: take the compiled code and package it in its distributable format, such as a JAR.

4. mvn clean: attempts to clean a project's working directory of the files that we're generated at build-time

5.mvn install: used to automatically install the project's main artifact (the JAR, WAR or EAR), its POM and any attached artifacts (sources, javadoc, etc) produced by a particular project.


