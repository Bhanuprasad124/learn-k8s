pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                // Must be inside node to access workspace
                script {
                    node {
                        git branch: 'main',
                            credentialsId: '87a6ce60-2b39-49d1-b657-1ec198812d72',
                            url: 'https://github.com/Bhanuprasad124/learn-k8s.git'
                    }
                }
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running...'
            }
        }
    }
}
