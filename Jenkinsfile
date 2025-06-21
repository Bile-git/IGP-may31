pipeline
{
	agent any
	stages
	{
		stage('Code Checkout')
		{
			steps
			{
				git branch: 'main',
                                       url: 'https://github.com/Bile-git/IGP-may31.git'
			}
		}
		
		stage('Code Compile')
		{
			steps
			{
				sh 'mvn compile'
			}
		}

		stage('Unit Test')
		{
			steps
			{
				sh 'mvn test'
			}
		}

		stage('Code packaging')
		{
			steps
			{
				sh 'mvn package'
			}
		}
   }
}

