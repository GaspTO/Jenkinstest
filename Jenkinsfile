pipeline {
    agent any

    options { skipDefaultCheckout() }
    
    stages {
        stage('Hello') {
            steps {
                sh 'cat example.txt'
            }
        }
    }
}

