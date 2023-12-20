pipeline {
    agent any

    stages {
       
        stage('Run Python Script') {
            steps {
                // Execute the Python script
                sh 'python hello_chatgpt.py'
            }
        }
    }

    post {
        always {
            // Clean up or post-execution steps if necessary
            echo 'Python script execution completed.'
        }
    }
}