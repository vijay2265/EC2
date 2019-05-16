pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    }
 }  
