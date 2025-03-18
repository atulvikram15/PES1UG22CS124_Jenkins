pipeline {
    agent any

    stages {
        stage('Build') {
    steps {
        script {
            sh 'pwd'  
            sh 'ls -la'  
            sh 'g++ -o PES1UG22CS124-1 main.cpp'  
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
