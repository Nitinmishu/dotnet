def response = "None"

pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                echo 'Stage 1'
            }
        }

        stage('Build') {
            steps {
                sh 'sudo apt-get install awscli -y'
            }
        }

        stage('Prepare all yml files') {
            steps {
                sh 'aws s3 ls s3://donet-build'
            }
        }

        stage('Run Deployment Script EmpNpsMS') {
            steps {
                echo 'Stage 4'
            }
        }
    }
}