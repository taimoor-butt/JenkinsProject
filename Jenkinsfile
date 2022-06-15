pipeline {
    agent any
    stages {
        stage('mvn clean') {
            steps {

                bat "mvn clean JenkinsProject"
            }
        }
        stage('install') {
            steps {
                bat "mvn install JenkinsProject"
            }
        }
        stage('test') {
            steps {
                bat "mvn test JenkinsProject"
            }
        }
        stage('package') {
            steps {
                bat "mvn package JenkinsProject"
            }
        }
    }
}