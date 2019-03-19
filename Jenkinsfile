pipeline {
    agent any
        stages {
            stage('First') {
                steps {
                    sh ' echo "Step One" '{
                        EXECUTE = "True"
                    }
                }
            }
 
 
            stage('Second') {
                when {
                environment name: 'EXECUTE', value: 'True'
                     }
                steps {
                    sh ' Updating Second Stage '
                }
            }
 
            stage('Third') {
                steps {
                    sh ' echo "Step Three" '
                }
            }
        }
}
