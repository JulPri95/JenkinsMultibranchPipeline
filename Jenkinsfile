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
				when {
               			 branch 'First'
				environment name: 'EXECUTE', value: 'True'
            				steps {											
						echo "Step Two"	
						echo "Updating Second Stage"
					}	}		
				} 			
			stage('Third') {				
				steps {											
						echo "Step Three"				
					}			
				}		
			}
		}
