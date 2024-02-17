pipeline { 
  
   agent any

   stages {
   
     stage('Check Git Version') { 
        steps { 
           git --version
        }
     }
     
     stage('Check Java Version') { 
        steps { 
           java --version
        }
      }

         stage("check current location) { 
         steps { 
           pwd
         }

     }
  
   	}

   }
