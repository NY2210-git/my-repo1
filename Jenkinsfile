pipeline {
    
	   agent {
	           
			    label 'built-in'
				
				}
				  
				 stages  {

                    stage ('apache-1') {   				 

                            steps {
                    
                           sh "yum install httpd -y"
                          }
 
                  }
				  
				  stage ('apache-start'){
				      
					         steps {
						 
						           sh "service httpd start"
						 }
						 
					}
       
                  stage ('var-file'){

                       steps {
                 
				     sh "cp -r index.html /var/www/html"
                     sh "chmod -R 777 /var/www/html/index.html"					  
						 
                    }

                }
           
            }		   
	
   
   
   
   
   }
