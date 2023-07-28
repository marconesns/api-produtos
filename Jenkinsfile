pipeline {

    agent any

    stages {
        stage ('Build Image') {
            agent { dockerfile true
            docker {
                image: 'marconesns/api-produtos:v1.0'
            }
        }
            steps {
                echo "Teste de msg"
            }
       }
}
}