pipeline {
    agent any

    stages {
        stage("Init"){
            steps {
               echo "init step"
               bat 'npm install'
            }
        }
        stage("Testing"){
            steps {
               echo "testing step"
               bat 'npm test'
            }
        }
        stage("Running"){
            when {
                expression {
                    env.BRANCH_NAME == 'main'
                }
            }
            steps {
               echo "we are back in buisness ${currentBuild.result}"
            }
        }
         stage("Running"){
            when {
                expression {
                    env.BRANCH_NAME != 'main'
                }
            }
            steps {
               echo "we are back in NOT buisness ${currentBuild.result}"
            }
        }

    }
}