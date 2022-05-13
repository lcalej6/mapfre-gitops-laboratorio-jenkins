pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Segundo Stage') {
            agent {label 'docker-agent'}
            steps {
                sh 'echo "Hello World"'
                sh '''
                    hostname
                    pwd
                    ls -la
                '''
            }
    }
}
