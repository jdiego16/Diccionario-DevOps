<div>
<p style = 'text-align:center;'>
<img src="https://www.sonarqube.org/assets/logo-31ad3115b1b4b120f3d1efd63e6b13ac9f1f89437f0cf6881cc4d8b5603a52b4.svg" alt="sonar" width="700px">
</p>
</div>

# Definition

>is an open source platform for continuous inspection of code quality through different static source code analysis tools. It provides metrics that help improve the quality of a program's code by allowing development teams to track and detect bugs and security vulnerabilities to keep the code clean.

## common terms
* Quality Gate: 
> are a series of conditions that the project under analysis must meet in order to proceed to the next stage.
* Code smells: 
>is an indication that parts of the code are not being written well, usually maintainability problems.
* Coverage:
> is a measure of the percentage of code that has been validated by tests.
* Quality Profiles: 
>is a central component where a set of rules are defined that when violated pose problems in the code base.
* Rules 
>SonarQube executes rules in the source code to generate issues.

## Features
* detects difficult problems
* analyzes the source code of more than 20 languages
* installs a local server which can be configured with different databases to analyze large amounts of code.

## requirements
* Sonarqube v.7.9.x
* SonarScaner
* plugin C++
* plugin R
* Quality profiles
* java version 11
## installation

1. download Sonarqube and SonarScaner from the official website (https://www.sonarqube.org/downloads/), also download plugins from Github (https://github.com/SonarOpenCommunity/sonar-cxx/releases/tag/cxx-2.0.6).
2. create the path to the pc disk location (C:\Sonar)
3. Extract the resources in the created path
4. open the location (C:\sonarsonarqube-x.x.x\windows-x86-64) from there run cmd.
5. execute the command ./StartSonar.bat
6. the default service runs on http://localhost:9000 and can be accessed on a web server
7. default login parameters are user admin and password admin
8. to install the plugins, you must copy the .jar files to the (C:\sonarsonarqube-x.x.x\extensions\plugins) and restart the service.