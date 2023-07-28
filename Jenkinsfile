pipeline {

    agent any

    stages {

        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("192.169.0.120:5000/marcones/api-produto", '-f ./src/Dockerfile ./src')
                    // dockerapp = docker.build("fabricioveronez/api-produto:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}