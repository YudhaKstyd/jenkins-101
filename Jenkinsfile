pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                container('dind'){
                    echo "Building.."
                    sh '''
                    docker build . -t yud-testing
                    '''
                }
            }
        }
        stage('Tes'){
            steps {
                container('dind'){
                    sh '''
                    docker image ls
                    '''
                }
            }
        }
    }
}