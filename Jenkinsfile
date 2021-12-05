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
                dir(path: './LibraryApp/LibraryApp'){
                    sh 'dotnet build LibraryApp.csproj'
                }
            }
        }

        stage('Prepare all yml files') {
            steps {
                sh 'pwd;ls -l;/usr/bin/aws s3 ls s3://donet-build'
            }
        }

        stage('Run Deployment Script EmpNpsMS') {
            steps {
                echo 'Stage 4'
            }
        }
    }
}