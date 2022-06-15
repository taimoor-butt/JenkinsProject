pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                bat "rmdir  /s /q JenkinsProject"
                bat "git clone https://github.com/taimoor-butt/JenkinsProject.git"
                bat "mvn clean -f JenkinsProject"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f JenkinsProject"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f JenkinsProject"
            }
        }
    }
}