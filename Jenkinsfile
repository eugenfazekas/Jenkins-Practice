pipeline {
    agent any

    stages {
        stage('docker-compose up') {
            steps {
              bat  'docker-compose up' 
            }
        }
		stage('docker-compose down') {
            steps {
              bat  'docker-compose down --remove-orphans' 
            }
        }
    }
}