pipeline {
    agent { 
        node {
            label 'jenkins-jenkins-agent'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                python3 --version
                pip3 --version
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''

                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}