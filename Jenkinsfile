pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '<your_build_command>'
            }
        }
        stage('Test') {
            steps {
                bat '<your_test_command>'
            }
        }
        stage('Deploy') {
            steps {
                bat '<your_deploy_command>'
            }
        }
    }
}
