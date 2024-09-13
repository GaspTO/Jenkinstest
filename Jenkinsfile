pipeline {
    agent any

    options { skipDefaultCheckout() }
    
    stages {
    	stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']],
                          userRemoteConfigs: [[name: 'jenkins_toast', url: 'git@github.com:GaspTO/Jenkinstest.git']]])
            }
        }	
    
        stage('Hello') {
            steps {
                sh 'cat example.txt'
            }
        }
    }
}

