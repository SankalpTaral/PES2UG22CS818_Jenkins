pipeline {
    agent any  // Allocate any available agent

    stages {
        stage('Build') {
            steps {
                script {
                    // Create a new working .cpp file
                    sh 'main.cpp'

                    // Optional: Add build commands here (replace with your build steps)
                    // echo 'Building the application...'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Optional: Add test commands here (replace with your test runner)
                    // echo 'Running unit tests...'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Optional: Add deployment commands here (replace with your deployment steps)
                    // echo 'Deploying to production...'
                }
            }
        }
    }

    // Post-condition: Display "pipeline failed" on any error
    post {
        always {
            echo 'Pipeline execution completed.'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
