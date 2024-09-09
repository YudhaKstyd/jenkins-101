pipeline {
    agent any { 
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                container('dind'){
                    echo "Building.."
                    sh '''
                    docker
                    '''
                }
            }
        }
}