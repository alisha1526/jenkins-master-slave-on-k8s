pipeline
{
	agent
	{
		label 'maven-slave'
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