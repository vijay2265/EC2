pipeline {
    agent {
        // Define agent details here
    }
    environment {
        AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    }
     stages {
        stage('Build') {
            steps {
                sh 'ansible-playbook EC2.yml'
            }
        }
    }
}    
