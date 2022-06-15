pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "https://github.com/taimoor-butt/JenkinsProject.git"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f JenkinsProject"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f JenkinsProject"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f JenkinsProject"
            }
        }
    }
}