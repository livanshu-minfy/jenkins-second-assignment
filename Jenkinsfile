pipeline {
    agent any

    stages {
        stage('Build Image') {
            steps {
                script {
                    sh 'docker build -t greet-app .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run greet-app'
                }
            }
        }
    }
}
