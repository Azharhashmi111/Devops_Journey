pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Azharhashmi111/Devops_Journey'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cp target/*.war /var/lib/tomcat9/webapps/'
            }
        }
    }
}

