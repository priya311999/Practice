pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                echo "building an application"
            }
        }
        stage('Test'){
            steps {
                echo "testing"
            }
        }
        stage('Deploy') {
            steps {
               echo "Deploying"
            }
        }
    }
}
