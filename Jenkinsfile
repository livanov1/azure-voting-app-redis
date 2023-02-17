@Library('https://github.com/livanov1/demo-shared-pipeline@master') _ 
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
    }
}