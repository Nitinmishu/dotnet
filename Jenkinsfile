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
                echo 'Stage 2'
            }
        }

        stage('Prepare all yml files') {
            steps {
                echo 'Stage 3'
            }
        }

        stage('Run Deployment Script EmpNpsMS') {
            steps {
                echo 'Stage 4'
            }
        }
    }
}