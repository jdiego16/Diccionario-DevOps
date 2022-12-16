pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'echo Hello World'
            }
        }
        stage('sleep') {
            steps {
                sh 'sleep 10'
            }
        }
        stage('Hello2') {
            steps {
                sh 'echo Hello World from jenkins file'
            }
        }
    }
}