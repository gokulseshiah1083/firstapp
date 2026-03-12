pipeline {
    agent any
    environment {
        // This is a common variable name for many applications like Spring Boot
        SERVER_PORT = '8082' 
    }
    stages {
        stage('Build') {
            steps {
                bat 'echo "Starting the maven clean package"'
                bat './mvnw clean package'
            }
        }
        stage('Run') {
            steps {
                bat 'echo "Starting the spring boot app"'
                bat './mvnw spring-boot:run'
            }
        }
    }    
}
