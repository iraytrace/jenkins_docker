pipeline {
  
	agent {
		docker { 
			label 'VSL_build'
			image 'lee:latest'
			// from https://confluence.di2e.net/display/DEVTOOLS/Jenkins+-+How+do+I#Jenkins-HowdoI-UseDockerinJenkins
			// registryUrl 'https://docker-di2e.di2e.net'
			// registryCredentialsId '687110ca-29bc-48c6-b35a-50b6040f1260'
		}
	}
  
	options { skipDefaultCheckout() }  // Only build agent gets source code. 

	stages {
		stage ('Build') {
			steps {
				bat 'echo hello lee'
				bat 'hostname'
				bat 'dir C:/'
				bat 'echo %CD%'
				bat 'wmic logicaldisk get caption,providername,drivetype,volumename'

			}
		}
	}
}
