pipeline {
    agent any

    stages {
        stage('Task 1: Checkout') {
            steps {
                // Task 1: Pulls the latest commit from your GitHub repository
                checkout scm
            }
        }

        stage('Task 2: Create output.txt') {
            steps {
                // Task 2: Uses the BAT 'echo' command and '>' to create a file
                bat "echo Welcome to Version 3 - File Creation > output.txt"
            }
        }

        stage('Task 3: Display File Content') {
            steps {
                // Task 3: Uses the BAT 'type' command to show the file contents
                bat "type output.txt"
            }
        }
    }
}
