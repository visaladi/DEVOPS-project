pipeline {
    agent any

    stages {
        stage('Move to frontend directory') {
            steps {
                script {
                    sh 'cd /var/lib/jenkins/workspace/Blogfinity-CI/blogfinity/frontend'
                }
            }
        }

        stage('Install Packages for frontend') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Fix Issues in frontend') {
            steps {
                script {
                    sh 'npm audit fix'
                }
            }
        }
    }
}

tools {
    nodejs "nodejs"
}