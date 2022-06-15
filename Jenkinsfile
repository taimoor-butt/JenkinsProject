pipeline {
    agent any
    stages {
        stage('mvn clean') {
            steps {
                bat "mvn clean JenkinsTest"
            }
        }
        stage('install') {
            steps {
                bat "mvn install JenkinsTest"
            }
        }
        stage('test') {
            steps {
                bat "mvn test JenkinsTest"
            }
        }
        stage('package') {
            steps {
                bat "mvn package JenkinsTest"
            }
        }
    }
}