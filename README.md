# Gradle Based Java Project Setup Guide
A step-by-step guide explaining how to setup a new Gradle based Java project without relying on IDE

- Go to section "Installing Gradle" in the document tab of the official gradle website (https://docs.gradle.org/current/userguide/installation.html), and read the instructions
- As of now, November 2018, the version of document is 4.10.2, and the prerequisite of the Java SDK version 7 or higher and the example is showing **java version "1.8.0_151"**. In fact, it seems that when Java SDK version 9 was used, it seemed that the gradle did not work properly, if I recall correctly.
- So, the very first step should be installing Java SDK first.
- Note that multiple versions of Java SDKs can be installed side-by-side, however, the Java path needs to be changed each time when you to run non-gradle Java 9 environment or the gradle-based project.
- Managing the Java path can be confusing or problematic due to the recent change by JDK 9.
  - Java 9: C:\ProgramData\Oracle\Java\javapath
    - Java 9 use UNIX like link Windows filesystem junction, which points to the actual directory
    - The caveat is reported and discussed in the following blog: http://marxsoftware.blogspot.com/2015/07/windows-oracle-java-path.html
  - Java 8: D:\Java\jdk1.8.0_181\bin
    - Note that Java 8 SE public updates will end after January 2019 for Commercial User and December 2020 for Personal User
- Chocolatey, "the package manager for Windows", is recommended from the gradle website, and it is easy to use, however, changing the installation location is not an easy task unfortunately. For example, if you have a separate "D" drive for larger space disk, this will be a pain.
