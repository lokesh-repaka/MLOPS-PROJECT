pipeline {
    agent any
    
    stages {
        stage('cloning from github repo') {
            steps {
                script {
                    echo 'cloning from github repo.........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'mlops-github-token', url: 'https://github.com/lokesh-repaka/MLOPS-PROJECT.git']])
                }
            }
        }
    }
}