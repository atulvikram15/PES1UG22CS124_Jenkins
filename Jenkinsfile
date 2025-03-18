pipeline {
    agent any

    stages {
        stage('Build') {
    steps {
        script {
            sh 'pwd'  # Print current workspace path
            sh 'ls -la'  # List all files
            sh 'g++ -o PES1UG22CS124-1 main.cpp'  // Compile
        }
    }
}

        stage('Test') {
            steps {
                script {
                    sh './PES1UG22CS124-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
