pipeline{

	agent{
		docker{image  'javiersantos/android-ci:latest'}

	}
	stages{
		stage('Compile'){
			steps{
				echo "Hello World"
				sh './gradlew clean build'
			}
		}

	}
}