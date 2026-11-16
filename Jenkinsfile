pipeline {
    agent any

    stages {
        stage('Diagnose Environment') {
            steps {
                sh '''
                    echo "=== HOSTNAME ==="
                    hostname

                    echo "=== USER ==="
                    id

                    echo "=== WORKSPACE ==="
                    pwd

                    echo "=== DOCKER FILE ==="
                    ls -l /usr/bin/docker || true

                    echo "=== ROOT DIRECTORY ==="
                    ls -la /

                    echo "=== PROCESS CONTAINER ==="
                    cat /proc/1/cgroup || true
                '''
            }
        }
    }
}