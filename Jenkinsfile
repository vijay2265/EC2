pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'env'
            }
        }
         stage('Deploy') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    }
}    
