@Library('https://github.com/livanov1/demo-shared-pipeline') _ 
pipeline {
    agent any
    stages {
        stage('call library'){
            steps {
                script {
                    helloWorld()
                }
            }
        }
        stage('Testing'){
            steps{
                echo 'This should be out there in the console'
            }
        }
    }
}