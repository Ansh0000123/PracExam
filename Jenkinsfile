pipeline {
    agent any

    parameters {
        string(name: 'PROJECT_NAME', defaultValue: 'MyProject', description: 'Project name')
        choice(name: 'ENVIRONMENT', choices: ['staging', 'production'], description: 'Deployment environment')
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code for project: ${params.PROJECT_NAME}"
            }
        }

        stage('Build') {
            steps {
                echo "Building project: ${params.PROJECT_NAME}"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests for project: ${params.PROJECT_NAME}"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${params.PROJECT_NAME} to ${params.ENVIRONMENT} environment"
            }
        }
    }
}
