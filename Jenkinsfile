pipeline {
    agent any
    tools {
        nodejs "nodejs"  // Имя инструмента Node.js
    }
    stages {
        stage('Verify Node.js Version') {
            steps {
                sh 'node -v'   // Проверяем установленную версию Node.js
                sh 'npm -v'    // Проверяем установленную версию npm
            }
        }
        stage('Checkout') {
            steps {
                git branch: 'main', credentialsId: 'github-dock', url: 'git@github.com:Esstie/tired.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'  // Устанавливаем зависимости с помощью npm
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
