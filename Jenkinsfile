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
                 echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        stage('psuh to dockerhub') {
            steps {
                echo 'Deploying....'
                sh 'docker push yeshwanthjavvaji/knote:${BUILD_NUMBER}'
            }
        }
    }
}