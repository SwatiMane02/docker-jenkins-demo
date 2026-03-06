pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh '/usr/local/bin/docker build -t myapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh '/usr/local/bin/docker run -d -p 8081:80 myapp'
            }
        }

    }
}
