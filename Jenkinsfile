pipeline {
    agent any
    parameters {
        // Task 2: Accept USERNAME parameter from the user
        string(name: 'USERNAME', defaultValue: 'Guest_User', description: 'Please enter your username')
    }
    stages {
        stage('Task 1: Checkout') {
            steps {
                // Task 1: Checkout latest version from GitHub
                checkout scm
            }
        }
        stage('Task 3: Create user.txt') {
            steps {
                // Task 3: Create user.txt and store the parameter inside it
                bat "echo ${params.USERNAME} > user.txt"
                echo "Username '${params.USERNAME}' has been saved to user.txt"
            }
        }
        stage('Verify File') {
            steps {
                // Optional: Verify the content in the console
                bat "type user.txt"
            }
        }
    }
}
