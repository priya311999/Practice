pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                echo "building"
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
        post{
            always{
                emailext body: 'Summary', subject: 'Pipe Notify', to: 'rapr.priya31@gmail.com'
            }
        
        }
    }
}
