pipeline {
    agent any
    tools {
    Nodejs 'nodejs 4.8.3'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'npm install'
                sh 'npm run test'
                sh 'npm run coverage'
            }
        }
        stage('Package') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
