pipeline {
    agent any

    // environment {
    //     AWS_REGION = 'us-east-1'
    //     ECR_REPO = 'my-repo'
    //     IMAGE_TAG = 'latest'
    //     SERVICE_NAME = 'llmops-medical-service'
    // }

    stages {
        stage('Clone GitHub Repo') {
            steps {
                script {
                    echo 'Cloning GitHub repo to Jenkins...'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/Keshav-chand/Medical-RAG-Chatbot.git']])
                }
            }
        }
    }
}
