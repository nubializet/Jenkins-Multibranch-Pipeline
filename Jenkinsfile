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
				
				echo "${EXECUTE}"
						
						
				      }		 

			stage('Three') {
						steps {
							sh ' echo "Step Three" '
							}
				       }
			}
}
