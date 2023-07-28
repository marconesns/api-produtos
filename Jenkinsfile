pipeline {

    agent any

    stages {
        stage ('Build Image') {
            docker {
                image: 'marconesns/api-produtos:v1.0'
            }
        }
            steps {
                echo "Teste de msg"
            }
       }
}