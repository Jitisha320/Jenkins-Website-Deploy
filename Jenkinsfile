pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Jitisha320/Jenkins-Website-Deploy.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    rm -rf /var/www/html/*
                    cp index.html style.css script.js /var/www/html/
                '''
            }
        }

    }
}
