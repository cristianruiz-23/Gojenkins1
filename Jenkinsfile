pipeline {
    agent { label 'agent3' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/cristianruiz-23/Gojenkins1.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}
