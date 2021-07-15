pipeline {
	agent any
	environment { EXECUTE = "default"
	}
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							script {
								EXECUTE = "True"
								}
							echo "${EXECUTE}"
							}	
				     }
						
		

			stage('Two') {
						when {
							environment { EXECUTE == "True" }							
						     }
						steps { 
							sh ' echo "Step Two" '
							sh ' echo "Updating Second Stage" '	
						      }
						
				      }		 

			stage('Three') {
						steps {
							sh ' echo "Step Three" '
							}
				       }
			}
}
