pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o pes1ug22cs304-1 main.cpp'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    sh './pes1ug22cs304-1'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deployment stage successfull (pes1ug22cs304'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
