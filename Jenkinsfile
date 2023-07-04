/* groovylint-disable NestedBlockDepth */
pipeline {
    agent any
    
    stages {
        stage('Build and Deploy') {
            parallel {
                stage('Metrics Management') {
                    steps {
                        bat 'echo "Hi This is First Stage - Metrics Management"'
                    }
                }

                stage('Tenant Management') {
                    steps {
                        bat 'echo "Hi This is Second Stage - Tenant Management"'
                    }
                }
                stage('ui-config Management') {

                    steps {
                        bat 'echo "Hi This is Third Stage - ui-config Management"'
                    }
                    }
                stage('user management') {
                    steps {
                        bat 'echo "Hi This is Fourth Stage - user Management"'
                    }
                }
                stage('Deploy DAGS') {
                     steps{
                         bat 'echo "Hi This is Fifth Stage - DAGS deployment Management"'
                    }
                }
            }
        }  
    }
}
