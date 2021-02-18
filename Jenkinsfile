pipeline {
    agent any
    
    stages {
        stage("Init"){
            steps {
                npm install
            }
        }
        stage("Testing"){
            steps {
                npm test
            }
        }
        stage("Running"){
            steps {
                npm start
            }
        }
    }
}