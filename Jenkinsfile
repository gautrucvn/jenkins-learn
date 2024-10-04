pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-token', url: 'https://github.com/gautrucvn/jenkins-learn.git'

            }
        }
    }
}
