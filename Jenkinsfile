pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'mkdir -p devops/target && echo "Sample app built" > devops/target/myapp.war'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying WAR to Tomcat...'
                sh 'sudo cp devops/target/*.war /var/lib/tomcat9/webapps/'
            }
        }
    }

    post {
        success {
            echo '✅ Deployment Successful!'
        }
        failure {
            echo '❌ Deployment Failed!'
        }
    }
}

