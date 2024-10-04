pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-account', branch: 'main', url: 'https://github.com/gautrucvn/jenkins-learn.git'
            }
        }
    }
}
