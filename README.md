Jenkins Slave image with Java 11, Skopeo and Maven 3.6.3
===================

Tools
-------------------
* Programming Language - Java
* Pipeline Script - Jenkins Script

Concept
--------------------
A simple Dockerfile for creating Jenkins Slave on Openshift. Consist of Java 11, Skopeo (for migrating images between image registry) and the latest Maven version, at this time is 3.6.3.

Can be set directly on Jenkins configuration, 
![jenkins slave jdk11](jenkins-slave-jdk11.png)

or imported to Openshift by using this command,
```
oc import-image docker.io/edwinkun/jenkins-slave-skopeo-jdk11-new --confirm
```