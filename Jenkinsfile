pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/pratik-baibhav/githubbasics.git'
            }
        }

        stage('Test') {
            steps {
                sh 'ls index.html'
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo cp *.html /var/www/html/'
            }
        }
    }
}
