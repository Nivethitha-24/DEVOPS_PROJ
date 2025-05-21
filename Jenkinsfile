pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git credentialsId: 'github-token', url: 'https://github.com/Nivethitha-24/DEVOPS_PROJ.git'
            }
        }

        stage('Deploy to Local Web Server') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
