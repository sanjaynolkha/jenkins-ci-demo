pipeline {
    agent any

    stages {

        stage('Checkout Info') {
            steps {
                echo 'Repository checked out successfully'
                sh 'git --version'
                sh 'ls -l'
            }
        }

        stage('Build Simulation') {
            steps {
                echo 'Simulating build step'
                sh 'echo Build started at $(date)'
            }
        }

        stage('Test Simulation') {
            steps {
                echo 'Simulating tests'
                sh 'echo All tests passed'
            }
        }

        stage('Environment Info') {
            steps {
                sh 'hostname'
                sh 'uname -a'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
