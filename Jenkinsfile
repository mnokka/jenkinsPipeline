pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the repository
                echo "checkout scm part."
            }
        }
        
        stage('Build') {
            steps {
                // Build the project using a shell script
                echo "Building the project..."
                echo "Build successful!"
            }
        }
        
        stage('Test') {
            steps {
                // Run a simple test using a shell script
                echo "Running tests..."
                echo "Tests passed!"
            }
        }
    }
    
    post {
        success {
            // This block executes if the Pipeline succeeds
            echo 'postbuild action: Pipeline succeeded!'
        }
        failure {
            // This block executes if the Pipeline fails
            echo 'postbuild action: Pipeline failed!'
        }
    }
}

