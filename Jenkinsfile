pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Your build steps here
                sh 'make' // Assuming your build process is to run a 'make' command
            }
        }
        stage('Test') {
            steps {
                // Your test steps here
                sh 'make test' // Assuming your test process is to run 'make test'
            }
        }
        stage('Deploy') {
            steps {
                // Your deployment steps here
                sh 'make deploy' // Assuming your deployment process is to run 'make deploy'
            }
        }
    }

    post {
        always {
            // Display 'pipeline failed' in case of any errors
            echo 'pipeline failed'
        }
    }
}
