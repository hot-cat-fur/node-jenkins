pipeline {
    agent any

    stages {
        stage("Init"){
            steps {
               echo "hello there"
            }
        }
        stage("Testing"){
            steps {
               sh 'npm test'
            }
        }
        stage("Running"){
            steps {
               echo "we are back in buisness ${currentBuild.result}"
            }
        }
    }
}