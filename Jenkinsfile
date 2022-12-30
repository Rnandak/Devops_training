pipeline{
	agent {docker {image 'maven:3.6.3-jdk-8'}}
		stages {
			stage('Build') {
				steps{
				 sh 'mvn --version'
				 echo "build"
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
