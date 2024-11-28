pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                // Add your build commands here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
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
