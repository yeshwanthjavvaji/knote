pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'docker build -t yeshwanthjavvaji/knote:${BUILD_NUMBER} .'
                sh 'docker images'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'docker ps'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}