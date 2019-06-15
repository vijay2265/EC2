pipeline {
    agent any
    stages {
         stage('Deploy') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    }
}    
