pipeline{

	agent any
	stages{
		 stage('Clean') {
     		 steps {
        		sh './gradlew clean'
     			}
		 }
		 stage('Build') {
     		 steps {
        		sh './gradlew assembleDebug'
     			}
		 }
		 stage('Unit test') {
     			 steps {
        			// Compile and run the unit tests for the app and its dependencies
       				 sh './gradlew testDebugUnitTest testDebugUnitTest'

       				 // Analyse the test results and update the build result as appropriate
       				 junit '**/TEST-*.xml'
     			 }
    	}
    	stage("fastlane"){
    	    steps{
    	          fastlane test
       	    }

    	}

	}
}
