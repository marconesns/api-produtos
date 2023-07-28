pipeline {

    agent any

    stages {

        stage ('Build Image') {
            steps {
                script {
                    // dockerapp = docker.build("marcones/api-produto:v1.0", '-f ./src/Dockerfile ./src')
                    sh 'docker build -t marcones/api-produtos:v1.0 -f ./src/Dockerfile'
                }
            }
        }
    }
}