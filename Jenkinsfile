pipeline {
    agent any
    environment {
        AWS_ACCESS_KEY_ID     = credentials('aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('aws-secret-access-key')
    }
    stages {
        stage('Build') {
            steps {
                sh 'env'
     stages {
        stage('Deploy') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    }
}    
