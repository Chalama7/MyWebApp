pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Build your application (e.g., Maven, Gradle)
                sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                // Run unit tests
                sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy to AWS or Azure
                sh 'aws s3 cp target/app.war s3://my-bucket/'
            }
        }
    }
}
