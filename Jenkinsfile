pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                sh "ls"
                sh "docker --version"
                sh "docker-compose --version"
                sh "workspace location: ${WORKSPACE}"
                sh "ls -al ${WORKSPACE}"


            }
        }
	    stage('Test'){
            steps {
                sh "pwd"
            }
	  }
        stage('Deploy'){
        steps {

            sh "cd /var/lib/jenkins/workspace/Basic Pipeline"
            sh "docker-compose up -d"
            sh "docker-compose ps"
        }
	  }
    }
}