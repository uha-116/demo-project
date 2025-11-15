pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/uha-116/demo-project.git'
            }
        }

        stage('Build') {
            steps {
                echo "Build step running..."
            }
        }

        stage('Test') {
            steps {
                echo "Test step running..."
            }
        }
    }

    post {
        success {
            echo "BUILD SUCCESS!"
        }
        failure {
            echo "BUILD FAILURE!"
        }
    }
}
