pipeline
{
	agent
	{
		label 'maven-slave'
	}
	
	tools
	{
		maven 'my_maven'
		jdk 'my_jdk'
	}
	
	stages
	{
		stage('Checkout Code')
		{
			steps
			{
				checkout scm
			}
		}

		stage('Build Code')
		{
			steps
			{
				sh 'mvn clean install'
			}
		}
	}
}
