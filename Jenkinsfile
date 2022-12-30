pipeline{
	// agent {docker {image 'maven:3.6.3-jdk-8'}}
	agent any
		stages {
			stage('Build') {
				steps{
				 //sh 'mvn --version'
				 echo "build_id - $env.BUILD_ID"
				 echo "build_number -$env.BUILD_NUMBER"
				}
			}
			stage('Test') {
				steps{
				 echo "Test"
				}
			}
			stage('Integration Test') {
				steps{
				 echo "Integration Test"
				}
			}
		}
		post{
				always{
				echo "always"
				}
				success{
				echo "success"
				}
				failure {
				echo "failure"
				}
		}
}
