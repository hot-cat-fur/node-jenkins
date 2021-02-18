pipeline {
    agent any

    stages {
        stage("Init"){
            steps {
               sh 'npm install'
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