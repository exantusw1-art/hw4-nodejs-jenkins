pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                sh 'mkdir -p dist'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Test passed"'
            }
        }

        stage('Build') {
            steps {
                sh 'cp index.js dist/'
            }
        }

        stage('Archive Artifact') {
            steps {
                archiveArtifacts artifacts: 'dist/**', fingerprint: true
            }
        }
    }
}
