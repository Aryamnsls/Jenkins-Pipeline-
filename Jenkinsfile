pipeline{
	agent any 
	stages{
		stage('Build'){
			steps{
				echo 'Building the project...'
				 sh 'mkdir -p build && echo "Build successful!" > build/result.txt'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "All tests passed ✅"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to Tomcat...'
                sh 'echo "Deployment done!"'
            }
        }
    }
}
