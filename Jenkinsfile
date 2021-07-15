pipeline {
	agent any
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							script {
								env.VARIABLE="value"
								}
							}
						}

			stage('Two') { 
						steps { 
							sh ' echo "Step Two" '
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
