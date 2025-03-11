pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'gpoiu++ -o PES2UG22CS0411 main.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './YOUR_SRN-1'
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
