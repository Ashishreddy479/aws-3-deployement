pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning Repository...'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t aws-3-tier-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 aws-3-tier-app'
            }
        }
    }
}
