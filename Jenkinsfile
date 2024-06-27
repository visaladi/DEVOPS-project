pipeline {
    agent any

    stages {
        stage('Install Packages') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Fix Issues') {
            steps {
                script {
                    sh 'npm audit fix'
                }
            }
        }
    }
}