<div>
<p style = 'text-align:center;'>
<img src="https://www.jenkins.io/images/logo-title-opengraph.png" alt="jenkins" width="600px">
</p>
</div>

# Definitions
>is an open source server for continuous integration. It is a tool used to compile and test software projects continuously, making it easier for developers to integrate changes in a project and deliver new versions to users. it can be used to automate all sorts of tasks related to building, testing, and delivering or deploying software.


## Continuous integration
>is a software development practice whereby developers merge code changes into a central repository on a periodic basis, after which automatic releases and tests are run. 

## plugins

> extends its functionality, they are applications that contain a set of features which help to improve other software.
 
 ## webhooks
>It is a communication system between applications, providing a simple solution for the exchange of data between web applications.
It works by sending http requests defined by the user, it sends a request.

## Jobs
>is the main unit of Jenkins, which is in charge of planning and executing tasks defined by a user. For example, a job would be in charge of: downloading code from repositories, building, testing and monitoring its execution.

# First steps
this is the main screen of the jenkins platform
<div>
<p style = 'text-align:center;'>
<img src="https://raw.githubusercontent.com/jdiego16/Diccionario-DevOps/Feature/images/Jenkins/Imagen1.jpg" alt="jenkins" width="600px">
</p>
</div>
there you start creating a new project.

<div>
<p style = 'text-align:center;'>
<img src="https://github.com/jdiego16/Diccionario-DevOps/blob/Feature/images/Jenkins/new%20task.png?raw=true" alt="jenkins" width="600px">
</p>
</div>

There you can see the different types of Jobs that can be created.

* Freestyle proyect
* pipeline
* multi-configuration project
* folder
* multibranch pipelinw
* organization folder


## pipeline
are a series of add-ons that allow the integration of elements related to continuous delivery,the parameters of its operation are written in a script under a defined syntax, you can also have files called "jenkinsfile" where the script of the developed pipeline will be contained.

example of pipeline script or jenkinsfile


<pre><code>pipeline {  (1)
    agent any  (2)
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { (3)
            steps { (4)
                sh 'make' (5) 
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit 'reports/**/*.xml' (6)
            }
        }
        stage('Deploy') {
            steps {
                sh 'make publish'
            }
        }
    }
}
</code></pre>

* (1). the block is declared with the expression "pipeline" containing all the instructions to execute.
* (2). In the declarative "agent" an executor is assigned on any of the available nodes.
* (3). is a scenario which contains a series of steps to be performed.
* (4). this declarative contains the steps to perform.
* (5). is a pipeline step which executes the command in the shell.
* (6). is another step taken by the JUnit plugin to add a test report.
## installation
>https://www.jenkins.io/doc/book/installing/


