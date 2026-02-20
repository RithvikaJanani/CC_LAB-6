pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("cc-lab6-backend", "backend")
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    docker.image("cc-lab6-backend").run()
                }
            }
        }
    }
}