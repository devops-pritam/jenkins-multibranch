stages {
    stage('parameter') {
        steps {
            script {
            
            properties([parameters([choice(choices: ['yes', 'no'], name: 'shouldWePrint')])])
                    }
              }
        
    
    }
    stage('Print') {
        when {
            expression { 
               return params.shouldWePrint == 'yes'
            }
        }
        steps {
                sh """
                java --version
                """
            }
        }
    stage('No Print') {
        when {
            expression { 
               return params.shouldWePrint == 'no'
            }
        }
        steps {
                echo 'No Print Required'
            }
        }
}


