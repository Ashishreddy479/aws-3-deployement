pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Ashishreddy479/aws-3-deployement.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t aws-3-tier-app .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'docker rm -f aws-container || true'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 --name aws-container aws-3-tier-app'
            }
        }
    }
}
