pipeline {
    agent any

    stages {
        stage('Echo declarative') {
            when {
                branch 'origin/master'
            }
            steps {
                echo "$GIT_BRANCH"
                echo "this is a master branch"
            }
        }
        stage('Most probably not master branch'){
            steps{
                script{
                    if(env.BRANCH_NAME == 'son'){
                        echo 'This is not my son'
                    } else {
                        echo 'This is the master bracnh prolly'
                    }
                }
            }
        }
    }
}
