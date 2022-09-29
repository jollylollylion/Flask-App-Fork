pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                sh "docker --version"
                sh "docker-compose --version"
                sh "workspace location: ${WORKSPACE}"

            }
        }
	    stage('Test'){
            steps {
                sh "pwd"
            }
	  }
        stage('Deploy'){
        steps {

            sh "cd 'Task 2/'"
            sh "docker-compose up -d"
            sh "docker-compose ps"
        }
	  }
    }
}