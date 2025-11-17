pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: 'TOKEN', url: 'git@github.com:RAVITEJA3929/newrepo.git'
            }
        }
        stage('List Directory') {
            steps {
                sh 'ls'
            }
        }
        stage('Sleep') {
            steps {
                sh 'sleep 10'
            }
        }
        stage('Run app.py') {
            steps {
                sh 'python3 app.py Ravi 25'
            }
        }
    }
}
