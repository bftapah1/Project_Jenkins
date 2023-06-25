pipeline {
    agent any
    // environment 
    //    DOCKERHUB_CREDENTIALS=credentials(docker-creds)

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t melong123/webapp:1.0.1 .'
            }
        }
        stage('Login') {
            steps {
                sh 'docker login -u melong123 -p melong123'
            }
        }
        stage('Push') {
            steps {
                sh 'docker push melong123/webapp:1.0.1'
            }
        }
    }
}