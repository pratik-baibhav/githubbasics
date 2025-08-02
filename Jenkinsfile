pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/pratik-baibhav/githubbasics.git'
            }
        }
        stage('Test') {
            steps {
                sh 'ls index.html'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/'
            }
        }
    }
}
