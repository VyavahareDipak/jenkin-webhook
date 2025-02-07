pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch:"main" , url: 'https://github.com/VyavahareDipak/jenkin-webhook.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Application') {
            steps {
                sh 'node app.js &'
            }
        }
    }
}
