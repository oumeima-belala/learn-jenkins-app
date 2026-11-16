pipeline {
    agent any

    stages {
        stage('Check Docker') {
            steps {
                sh '''
                    echo "Checking Docker..."
                    whoami
                    echo $PATH
                    ls -l /usr/bin/docker
                    command -v docker
                    docker --version
                '''
            }
        }
    }
}