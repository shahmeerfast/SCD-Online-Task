pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/shahmeerfast/SCD-Online-Task'
            }
        }

        stage('Run') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
