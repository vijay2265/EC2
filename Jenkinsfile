pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    } 
         stage('Build') {
            steps {
                // Example AWS credentials
                withCredentials(
                [[
                    $class: 'AmazonWebServicesCredentialsBinding',
                    accessKeyVariable: 'AWS_ACCESS_KEY_ID',
                    secretKeyVariable: 'AWS_SECRET_ACCESS_KEY'
                ]])
            }               
        }
    }
