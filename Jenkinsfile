pipeline {	
	agent any		
		stages {			
			stage('First') {				
				steps {	
					echo "Step One"	
					script{
						env.EXECUTE="True"
					}
					}			
				}			
			stage('Second') {				
            				steps {	
						echo "Step Two"	
						echo "Updating Second Stage"
						script {
							echo $(EXECUTE)
						}
					}		
				} 			
			stage('Third') {				
				steps {											
						echo "Step Three"				
					}			
				}		
			}
		}
