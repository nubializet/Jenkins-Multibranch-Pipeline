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
							sh ' echo "Step Two" '
							
						     }
						
				      }		 

			stage('Three') {
						steps {
							sh ' echo "Step Three" '
							}
				       }
			}
}
