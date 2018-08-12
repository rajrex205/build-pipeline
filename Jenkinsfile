pipeline {

      agent any

            stage {
	 
	         stage (' compile stage') {

	               steps {
	                 withmaven(maven : 'maven_3_5_0' ) {
		                 sh 'maven clean compile'
		  
		  }

	      }
	      
	  }
 
         	  stage ('test stage') {
	  
	             steps {
	                  withmaven(maven : 'maven_3_5_0'){

                             sh 'maven test' 

		 }
	      
	      }

	   }

	          stage ('code build') {
		     steps{
	             withmaven (maven : 'maaven_3_5_0') {
                              sh 'maven build'
          

	      }

	     }
	   }
    }   

}

