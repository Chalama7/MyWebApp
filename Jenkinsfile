pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
               bat 'copy target/*.war C:/Program Files/apache-tomcat-9.0.85\webapps\mvnwebapp\META-INF\maven\jenkins.mvn.demo\mvnwebapp'

            }
        }
    }
}
