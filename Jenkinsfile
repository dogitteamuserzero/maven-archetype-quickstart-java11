pipeline {
  agent any
  stages {
    stage('Fetch code') {
	  steps {
	    git branch: 'master', url: 'https://github.com/EmilianoFraga/maven-archetype-quickstart-java11.git'
	  }
	} 
	stage('Build') {
	  steps {
	    sh 'mvn clean install'
	  }
	}
	stage('Test') {
	  steps {
	    sh 'mvn test'
	  }
	}
  }
}
