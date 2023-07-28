pipeline {

    agent any

    stages {

        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("localhost:5000/marcones/api-produto:v1.0", '-f ./src/Dockerfile ./src')
                    // dockerapp = docker.build("fabricioveronez/api-produto:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}