pipeline {
    agent any
    stages {
        stage(‘Dcoker Build') {
            steps {
                echo 'Building..'
                sh 'docker build -t yeshwanthjavvaji/knote:${BUILD_NUMBER} .'
                sh 'docker images'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
