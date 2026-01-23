pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Building the application..."
            }
        }
        stage("Test") {
            steps {
                echo "Running unit tests..."
            }
        }
    }
    post {
        always {
            echo "I run no matter what happens!"
        }
    }
}
