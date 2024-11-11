pipeline {
    agent any
	 tools {
        nodejs "nodejs"  // Это имя настроенного инструмента Node.js в Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', credentialsId: 'github-dock', url: 'git@github.com:Esstie/tired.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
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
