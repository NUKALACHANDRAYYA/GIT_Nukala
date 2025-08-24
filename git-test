pipeline {
    agent any

    stages {
        stage('Check Host Docker & OS') {
            steps {
                echo 'Checking host Docker version and OS info...'
                sh '''
                    echo "Docker Version:"
                    docker version

                    echo "Host OS Info:"
                    cat /etc/os-release || uname -a
                '''
            }
        }
    }
}