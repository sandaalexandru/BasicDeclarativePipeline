pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/octocat/Hello-World.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Replace with actual build command, e.g., sh 'npm run build' or mvn compile
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace with actual test command, e.g., sh 'npm test' or mvn test
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully! ✅'
        }
        failure {
            echo 'Pipeline failed ❌'
        }
    }
}
