pipeline {
    agent any
    stages {
        stage('Checkout Source Code') {
            steps {
                checkout scm
                echo 'Successfully pulled code from the OmniFlow repository!'
            }
        }
        stage('Verify Server Environment') {
            steps {
                echo 'Checking installed tools...'
                sh 'docker --version'
                sh 'java -version'
            }
        }
        stage('Prepare Full-Stack Build') {
            steps {
                echo 'Pipeline ready to containerize and deploy Next.js/Node environments!'
            }
        }
    }
}
