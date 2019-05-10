pipeline{

	agent{
		docker{image 'javiersantos/android-ci:latest'}

	}
	stages{
		stage('Compile'){
			steps{
				sh './gradlew clean build'
			}
		}

	}
}