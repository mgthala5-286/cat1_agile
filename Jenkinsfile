pipeline {
    agent any
    parameters {
        // Task 3: Keeping the parameter for verification
        string(name: 'MESSAGE', defaultValue: 'Version 2 Test', description: 'Enter message')
    }
    stages {
        stage('Task 1: Checkout') {
            steps {
                // Task 1: Pulls the updated code you are pushing now
                checkout scm
            }
        }
        stage('Task 2: Display System Date') {
            steps {
                // Task 2: Windows command to show current date
                bat "date /t"
            }
        }
        stage('Task 3: Verify Parameter') {
            steps {
                // Task 3: Prints parameter again to verify it works in Version 2
                echo "Verified parameter value: ${params.MESSAGE}"
            }
        }
    }
}
