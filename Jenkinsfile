pipeline {

    agent any

    stages {

        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("localhost/marcones/api-produto", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}