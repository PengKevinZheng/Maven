# Maven

There are three things about Maven that are very nice.


1.Maven will (after you declare which ones you are using) download all the libraries that you use and and the libraries that they they use for you automatically. This is very nice, and makes dealing with lots of libraries ridiculously easy. This lets you avoid "depenendency hell". It is similar to Apache Ant's Ivy.

2.It uses "Convention over Configuration" so that by default you don't need to define the tasks you want to do. You don't need to write a "compile", "test", "package", or "clean" step like you would have to in Ant or a Makefile. Just put the files in the places Maven expects them and it should work off of the bat.

3.Maven also has lots of nice plug-ins that you can install that will handle many routine tasks from generating Java classes from an XSD schema using JAXB to measuring test coverage with Cobertura. Just add them to your pom.xml and they will integrate with everything else you want to do.