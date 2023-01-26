pipeline {
    agent any 

    stages {
        stage('build') {
            steps {
                sh """
                    docker compose -f docker-compose.yml -f docker-compose.dev.yml up -d --build
                """
            }
        }

        stage('test') {
            steps {
                echo 'deploying the test'
            }
        }
    }
}