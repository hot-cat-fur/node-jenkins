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
            steps {
               echo "we are back in buisness ${currentBuild.result}"
            }
        }
    }
}