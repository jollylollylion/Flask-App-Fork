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
            sh "cd /Task 2/"
            sh "ls -al"
            sh "docker-compose up -d"
            sh "docker-compose ps"
        }
	  }
    }
}