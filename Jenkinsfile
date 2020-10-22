pipeline {
    agent {
        label 'podman'
    }
    stages {
        stage('Build') {
            steps {
                //sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    /usr/sbin/ip a s
                '''
            }
        }
        stage('Test'){
            steps {
                sh '/bin/ping -c3 google.com'
            }
        }
    }
}

