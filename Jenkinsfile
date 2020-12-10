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
               			 // Only say hello if a "greeting" is requested
                			expression { EXECUTE == 'True' }
          			  }
            			steps {	
					echo "Step Two"	
					echo "Updating Second Stage"
					//script {
					//	echo "${EXECUTE}"
					//}
					}		
				} 			
			stage('Third') {				
				steps {											
						echo "Step Three"				
					}			
				}		
			}
		}
