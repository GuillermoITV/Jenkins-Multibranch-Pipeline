pipeline {
    agent any
        stages {
            stage('First') {
                steps {
                    script {
                      env.EXECUTE="True"
                    }
                }
            }
 
 
            stage('Second') {
                 when {
                environment name: 'EXECUTE', value: 'True'
                }
                steps {
                    sh ' echo "Success" '
                }
            }
 
            stage('Third') {
                when {
                environment name: 'EXECUTE', value: 'False'
                }
                steps {
                    sh ' echo "Step 3" '
                }
            }
        }
}
