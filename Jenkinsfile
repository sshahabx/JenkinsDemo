pipeline {
    agent any
    environment {
        FLAG = true  // Set the flag to control stage execution
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here
            }
        }
        stage('Test') {
            when {
                expression {
                    return FLAG == true  // Only run this stage if FLAG is true
                }
            }
            steps {
                echo 'Testing...'
                // Add your test commands here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment commands here
            }
        }
    }
    post {
        always {
            echo 'Post build condition running'
        }
        failure {
            echo 'Post action if build failed'
        }
    }
}
