pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t melong123/webapp:1.0.0 .'
            }
        }
    }
}