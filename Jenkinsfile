pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
              bat  'docker-compose up' 
            }
			post {
                always {
                    bat  'docker-compose down --remove-orphans'            
                }
            }
        }
    }
}