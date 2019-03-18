pipeline {
    agent any 
    stages {
        stage('Clone Repo and clean') {
            steps {
                sh "git clone https://github.com/jagadishwark/my-app.git"
                sh "mvn clean"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package"
            }
        }
    }
}


