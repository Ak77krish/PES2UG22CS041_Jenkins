pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'gpoiu++ -o PES2UG22CS041 main.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES2UG22CS041'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment stage (Placeholder)"
            }
        }
    }

    post {
        failure {
            echo "Pipeline failed"
        }
    }
}
