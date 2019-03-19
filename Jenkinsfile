pipeline {
    agent any
        stages {
            stage('First') {
                steps {
                    sh ' echo "Step 1" '{
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
                steps {
                    sh ' echo "Step 3" '
                }
            }
        }
}
