pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-account', branch: 'main', url: 'https://github.com/gautrucvn/jenkins-learn.git'
            }
        }

        stage('Build Docker') {
            withDockerRegistry(credentialsId: 'dockerhub', url: 'https://index.docker.io/v1/') {
                sh label: '', script: 'docker build -t rlucifer97/nodejs-test:v1'
                sh label: '', script: 'docker push rlucifer97/nodejs-test:v1'
            }
        }
    }
}
