pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Sjankatti/DevOps2026.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build required for static website'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}