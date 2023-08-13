#!groovy
pipeline {
	agent none
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:3.9-amazoncorretto-8'
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
  }
}
