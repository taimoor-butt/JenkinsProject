pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "git clone https://github.com/taimoor-butt/JenkinsProject.git"
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