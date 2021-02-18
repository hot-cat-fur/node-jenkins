pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }

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
               echo "we are back in buisness ${currentBuild.result}"
            }
        }
    }
}