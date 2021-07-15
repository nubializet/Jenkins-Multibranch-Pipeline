pipeline {
	agent any
	
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							script {
								env.EXECUTE = "True"
								}
							echo "${EXECUTE}"
							}	
				     }
		
			stage('Two') {
				steps{
					script {
						echo "${EXECUTE}"
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
