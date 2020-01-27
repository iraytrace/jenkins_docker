pipeline {
	agent { docker { 
			label 'VSL_build'
			image 'lee:latest'
	} }
	options { skipDefaultCheckout() }  // Only build agent gets source code. 
	stages { stage ('Build') { steps {
				bat 'echo hello lee'
				bat 'hostname'
				bat 'dir C:\\'
				bat 'echo %CD%'
				bat 'wmic logicaldisk get caption,providername,drivetype,volumename'
	} } }
}
