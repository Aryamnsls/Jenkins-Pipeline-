pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello Dosto!'
                sh 'mkdir -p devops'
                echo 'Mast Hoon!!'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // You can add real test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment steps later (like copying files or running a container)
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully ✅'
        }
        failure {
            echo 'Pipeline failed ❌'
        }
    }
}

