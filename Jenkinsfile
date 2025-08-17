pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/your-username/your-repo.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                echo 'No build step for static HTML, skipping...'
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo cp -r * /var/www/html/'  // Adjust path as needed
            }
        }
    }
}
