pipeline {	
	agent any		
		stages {			
			stage('First') {				
				steps {										
						echo "Step One"	
						env.EXECUTE="True"
					}			
				}			
			stage('Second') {				
            				steps {											
						echo "Step Two"	
						echo "Updating Second Stage"
					}		
				} 			
			stage('Third') {				
				steps {											
						echo "Step Three"				
					}			
				}		
			}
		}
