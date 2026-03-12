pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh './mvnw clean package'
            }
        }
        stage('Run') {
            steps {
                sh './mvnw spring-boot:run'
            }
        }
    }    
}
