pipeline {
    agent any
    stages {
        stage('Test') {
            steps{
                sh './gradlew clean'
                sh './gradlew test'
            }
        }

        stage('Build Project') {
            steps{
                sh './gradlew assembleDebug'
            }
        }
    }
}