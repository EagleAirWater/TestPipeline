	pipeline{
	agent any

	stages{
		stage('checkout'){
			steps{
				checkout scm
			}}
		stage('build'){
			steps{
				sh '/home/dhairya/devops/apache-maven-3.9.6-bin/apache-maven-3.9.6/bin/mvn install'
			}}
		stage('Deployment'){
			steps{
				sh 'cp target/TestPipeline.war /home/dhairya/devops/apache-tomcat-8.5.99/webapps/'
			}}
		}
}
