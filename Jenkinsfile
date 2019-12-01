pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                withAWS(credentials: 'aws-credentials', region: 'ap-south-1') {
                sh 'ansible-playbook EC2.yml'
                }
            }
        } 
    }
}    
