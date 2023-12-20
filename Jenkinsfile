pipeline {
    agent any

    stages {
       
        stage('Build') {
            steps {
                // Compile the Java code
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                // Run the compiled Java program
                sh 'java HelloWorld'
            }
        }
    }

    post {
        always {
            // Clean up any artifacts or temporary files if necessary
            sh 'rm -f HelloWorld.class'
        }
    }
}
