pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh './mvnw package'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'java -jar target/*.jar'
            }
        }
    }
}