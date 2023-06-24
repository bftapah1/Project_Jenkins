pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t melong123/webapp:1.0.1 .'
            }
        }
                stage('RUN') {
            steps {
                sh 'docker run -d --name my-webapp -p 88:80 melong123/webapp:1.0.1'
            }
        }
    }
}