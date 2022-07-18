pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([
                        parameters([
                            choice(
                                choices: ['Hivv_soe', 'Aem_soe', 'Res_soe'], 
                                name: 'SOE_PARAMETER'
                            )
                        ])
                    ])
                }
            }
        }
        stage('print parameters') {
            steps {
                script {
                    echo params.SOE_PARAMETER
                }
            }        
                    
        }       
    }   
}
