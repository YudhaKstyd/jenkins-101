pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                container('dind'){
                    echo "Building.."
                    sh '''
                    docker build -t testing:v1 .
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