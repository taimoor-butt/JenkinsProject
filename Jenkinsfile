pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "rm JenkinsProject"
                bat "git clone https://github.com/taimoor-butt/JenkinsProject.git"
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