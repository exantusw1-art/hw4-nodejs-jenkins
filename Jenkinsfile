pipeline {
    agent any
<<<<<<< HEAD

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'git@github.com:exantusw1-art/hw4-nodejs-jenkins.git'
            }
        }

=======
    stages {
>>>>>>> 4cc1a359c09ee76dd13ca3b5c151da76f59643d6
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }
<<<<<<< HEAD

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Archive Artifact') {
            steps {
                archiveArtifacts artifacts: 'dist/**', fingerprint: true
=======
        stage('Build') {
            steps {
                sh 'node index.js'
            }
        }
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '**/*', fingerprint: true
>>>>>>> 4cc1a359c09ee76dd13ca3b5c151da76f59643d6
            }
        }
    }
}
