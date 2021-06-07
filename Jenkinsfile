pipeline {
    agent any 
    environment {
        //once you sign up for Docker hub, use that user_id here
        registry = "aagupta942/currency-exchange-basic"
        //- update your credentials ID after creating credentials for connecting to Docker Hub
        registryCredential = 'dockerhub_id'
        dockerImage = ''
    }
    stages {
    	// Building Docker images
    	stage('Building image') {
      		steps{
        		script {
          			dockerImage = docker.build registry
        		}
      		}
    	}
	}
}