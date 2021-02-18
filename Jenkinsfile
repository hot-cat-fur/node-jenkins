pipeline {
    agent any

    stages {
        stage("Init"){
            steps {
               echo "init step"
               sh 'npm install'
            }
        }
        stage("Testing"){
            steps {
               echo "testing step"
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