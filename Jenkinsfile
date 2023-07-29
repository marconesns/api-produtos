pipeline {
    agent any
//  agent {
//         dockerfile true
//     }    

    stages {
        stage ('Build Image') {
            steps {
                script{
                    withDockerRegistry(credentialsId: '44d42ecb-f557-4e1c-8f26-b14b35c42856') {
                        sh "docker build -t marconesns/api-produtos:v1.0 ."
                        sh "docker push marconesns/api-produtos:v1.0"
                }
                } 
            }
       }
    }
}