pipeline {
	agent any
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							env.EXECUTE="True"
							}
						}

			stage('Two') { 
						steps { 
							sh ' echo "Step Two" '
							echo ${VARIABLE}
						    }
						}		 

			stage('Three') {
						steps {
							sh ' echo "Step Three" '
							}
						}
			}
}
