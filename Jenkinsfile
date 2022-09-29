pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                sh "ls"
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

            sh "cd ~/home/ubuntu/Flask-App-Fork/Task 2/"
            sh "docker-compose up -d"
            sh "docker-compose ps"
        }
	  }
    }
}