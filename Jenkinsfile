pipeline {
    agent any
    
    stages {
        stage('Build') {
            parallel {
                stage('MyMetrics-Management') {
                    steps {
                        bat 'echo "Hi This is First Stage - MyMetrics-Management"'
                    }
                }

                stage('MyTenant Management') {
                    steps {
                        bat 'echo "Hi This is Second Stage - MyTenant-Management"'
                    }
                }
                stage('My-ui-config Management') {

                    steps {
                        bat 'echo "Hi This is Third Stage - My-ui-config-Management"'
                    }
                    }
                stage('My-user-management') {
                    steps {
                        bat 'echo "Hi This is Fourth Stage - My-user-Management"'
                    }
                }
                stage('Deploying DAGS') {
                     steps{
                         bat 'echo "Hi This is Fifth Stage - My DAGS deployment Management"'
                    }
                }
            }
        }  
    }
}
