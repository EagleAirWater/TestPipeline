pipeline{
	agent any

	stages{
		stage{('checkout')
			steps{
				checkout scm
			}}
		stage{('build')
			steps{
				sh '/home/dhairya/devops/apache-tomcat-8.5.99/bin/mvn install'
			}}
		stage{('Deployment')
			step{
				sh 'cp target/TestPipeline.war /home/dhairya/devops/apache-tomcat-8.5.99/webapps/'
			}}
		}
}
