pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                sh "docker --version"
                sh "docker-compose --version"
            }
        }
	    stage('Test'){
            steps {
                sh "pwd"
            }
	  }
        stage('Deploy'){
        steps {
            dir('Task 2') {
                sh "pwd"
                sh "docker-compose up -d"
                sh "docker-compose ps"
            }
            sh "pwd"
        }
	  }
    }
    post {
        always {
            cleanWs()
        }
}