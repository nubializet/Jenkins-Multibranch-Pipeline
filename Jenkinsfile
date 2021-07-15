pipeline {
	agent any
	environment { EXECUTE = "default"
	}
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							script {
								env.EXECUTE = "True"
								
								}
							}	
				     }
						
		

			stage('Two') { 
						steps { 
							sh ' echo "Step Two" '
							sh ' echo "Updating Second Stage" '
							script {
								echo ${VARIABLE}
								}
						      }
				      }		 

			stage('Three') {
						steps {
							sh ' echo "Step Three" '
							}
				       }
			}
}
