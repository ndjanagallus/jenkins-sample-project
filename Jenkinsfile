pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add build commands here
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add test commands here
            }
        }

        stage('Env vars') {
          steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment commands here
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline succeeded! Notify or perform additional actions here.'
        }
        failure {
            echo 'Pipeline failed! Notify or perform additional actions here.'
        }
    }
}
