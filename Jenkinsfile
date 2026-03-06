pipeline {

    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Chaitanyaa1211/Docker-Jenkins-CICD.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t cicd-app .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'docker rm -f cicd-container || true'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 --name cicd-container cicd-app'
            }
        }

    }

}
