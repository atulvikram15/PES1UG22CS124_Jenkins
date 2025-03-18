pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG22CS124-1 main/main.cpp' 
            }
        }
        stage('Test') {
            steps {
                sh 'exit 1'  
            }
        }
    }
    post {
        failure {
            echo "Pipeline failed"
        }
    }
}
