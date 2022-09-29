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
            // sh 'cd pwd/Task 2/'
            sh "pwd"
            sh "ls -al"
            sh "docker-compose -f /Task 2/  up -d"
            sh "docker-compose -f /Task 2/ ps"
        }
	  }
    }
}