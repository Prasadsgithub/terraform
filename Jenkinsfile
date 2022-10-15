pipeline {
    agent  { label 'TRFM' }
    
    stages {
        stage('git clone') {
            steps {
               git url: 'https://github.com/Prasadsgithub/terraform.git',
               branch: 'main'
            }

        }
        stage('apply') {
            steps {
                sh 'terraform apply -auto-approve'
            }

        }
        
     }
}