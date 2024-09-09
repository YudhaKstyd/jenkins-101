pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                container('dind'){
                    echo "Building.."
                    sh '''
                    cd myapp
                    pip install -r requirements.txt
                    '''
                }
            }
        }
        stage('Tes'){
            steps {
                container('dind'){
                    echo "testing"
                    sh '''
                    cd myapp
                    python3 hello.py
                    python3 hello.py --name=Yud
                    '''
                }
            }
        }
    }
}