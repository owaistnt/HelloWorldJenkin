pipeline{

	agent any
	stages{
		stage('Compile'){
			steps{
				bat './gradlew clean'
				bat './gradlew build'
			}
		}

	}
}