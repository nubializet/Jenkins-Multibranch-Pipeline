pipeline {
	agent any
	stages { 
			stage('One') { 
						steps {
							sh ' echo "Step One" '
							script {
								env.EXECUTE="True"
								}
							}
						}

			stage('Two') { 
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
