pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/pratik-baibhav/my-static-site.git'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying static files to /var/www/html'
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}
