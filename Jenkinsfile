
pipeline {
	agent none
  stages {
  	stage('Install node') {
    	agent {
      	docker {
        	image 'node:16'
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
    stage('Docker Build') {
    	agent any
      steps {
      	sh 'docker build -t shanem/spring-petclinic:latest .'
      }
    }
  }
}