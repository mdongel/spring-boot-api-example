pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                sh 'java -version'
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
    }
}