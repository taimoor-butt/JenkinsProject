pipeline {
    agent any
    stages {
        stage('clean') {
            steps {
                bat "rm -rf JenkinsProject"
                bat "https://github.com/taimoor-butt/JenkinsProject.git"
                bat "mvn clean -f JenkinsProject"
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