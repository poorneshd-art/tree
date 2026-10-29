pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from version control...'
                // Add your git step here later, e.g.:
                // git 'https://github.com/your-repo/sample-project.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example for a Node.js or Java project:
                // sh 'npm install'
                // sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running automated tests...'
                // Example:
                // sh 'npm test'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check the logs.'
        }
    }
}
