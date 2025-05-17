pipeline {
    agent {
        docker {
            image 'node:18' // Official Node.js Docker image
            args '-p 3000:3000' // Optional: expose ports
        }
    }

    environment {
        NODE_ENV = 'development'
    }

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/shahmeerfast/SCD-Online-Task'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
