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
