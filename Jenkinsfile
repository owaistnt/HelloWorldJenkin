pipeline{

	agent{
		label 'android'
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