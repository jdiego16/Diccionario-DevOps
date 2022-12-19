<div>
<p style = 'text-align:center;'>
<img src="https://www.sonarqube.org/assets/logo-31ad3115b1b4b120f3d1efd63e6b13ac9f1f89437f0cf6881cc4d8b5603a52b4.svg" alt="sonar" width="700px">
</p>
</div>

# Definition

>is an open source platform for continuous inspection of code quality through different static source code analysis tools. It provides metrics that help improve the quality of a program's code by allowing development teams to track and detect bugs and security vulnerabilities to keep the code clean.

## static analysis
> is performed without running the software
## dynamic analysis
> it needs to run the software to be able to check its behavior at runtime



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

## Instance components
><div>
<p style = 'text-align:center;'>
<img src="https://docs.sonarqube.org/9.7/images/SQ-instance-components.png" alt="sonar1" width="700px">
</p>
</div>

## requirements
* Sonarqube v.7.9.x
* SonarScaner
* plugin C++
* plugin R
* Quality profiles
* java version 11

## rules
>SonarQube evalua el codigo fuente con un conjunto de reglas, las cuales estan basadas en estandares de programacion y buenas practicas. hay tres tipos de reglas:

* Code Smells (bad practices)
* Bug (code errors)
* Vulnerability ( errors affecting security)


the rules page is the entry point where the default rules for each language are stored or you can also create other templates based on the ones already established.

By default SonarQube installs a set of rules that apply to the commonly used languages.

With these default rules, the scanner analyzes the code in order to highlight potential errors.

## Quality profiles
>They define the set of rules to be applied during code analysis. Each project has a quality profile set for each supported language. When analyzing a project SonarQube determines which languages are used and uses the active quality profile for each of those languages in that specific project.


## installation

>https://docs.sonarqube.org/latest/setup/install-server/
