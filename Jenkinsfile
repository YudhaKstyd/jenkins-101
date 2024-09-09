pipeline {
    agent any
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
}