pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/susheelk3/jenkins-docker-demo.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('jenkins-docker-demo')
                }
            }
        }
    }
}
