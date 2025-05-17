pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/shahmeerfast/SCD-Online-Task'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
