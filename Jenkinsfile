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
				when {
                			expression { EXECUTE == 'True' }
          			  }
            			steps {	
					echo "Step Two"	
					echo "Updating Second Stage"
					}		
				} 			
			stage('Third') {
				when {
                			expression { EXECUTE == 'False' }
          			  }
				steps {											
					echo "Step Three"				
					}			
				}		
			}
		}
