pipeline {
    agent  { label 'TRFM' }
    
    stages {
        stage('git clone') {
            steps {
               git url: 'https://github.com/Prasadsgithub/terraform.git',
               branch: 'main'
            }

        }
        stage('init') {
            steps {
                sh 'terraform init'
            }

        }
        stage('apply') {
            steps {
                sh 'terraform apply -auto-approve'
            }

        }
        
     }
}