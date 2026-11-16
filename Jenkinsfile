pipeline {
    agent any

    stages {
        stage('Check Docker') {
            steps {
                sh '''
                    echo "Checking Docker..."
                    whoami
                    echo $PATH
                    which docker
                    docker --version
                '''
            }
        }
    }
}