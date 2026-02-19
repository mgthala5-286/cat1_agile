pipeline {
    agent any
    parameters {
        // Task 2: Define the MESSAGE parameter
        string(name: 'MESSAGE', defaultValue: 'Experiment 1: Version 1', description: 'Enter a custom message')
    }
    stages {
        stage('Task 1: Checkout') {
            steps {
                // Task 1: Verify GitHub integration
                checkout scm
            }
        }
        stage('Task 2: Print Parameter') {
            steps {
                // Task 2: Print the parameter value
                echo "The parameter value is: ${params.MESSAGE}"
            }
        }
        stage('Task 3: Execute BAT') {
            steps {
                // Task 3: Execute Windows batch command
                bat "echo Hello from Jenkins"
            }
        }
    }
}
