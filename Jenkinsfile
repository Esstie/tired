pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                  git branch: 'main', credentialsId: 'github-dock', url: 'git@github.com:Esstie/tired.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
