library 'https://github.com/livanov1/demo-shared-pipeline'

pipeline {
    agent any
    stages {
        stage('call library'){
            steps {
                script {
                    try {
                        helloWorld()
                    } catch (Exception) {
                        echo 'Exception occured: ' + e.toString()
                    } 
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