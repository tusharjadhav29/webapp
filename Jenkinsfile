pipeline {
    agent any
		tools
       {
			maven "Maven"
       }
	   
    stages {
		stage('checkout') {
           stage('SCM Checkout'){
                git url: 'https://github.com/tusharjadhav29/webapp.git',branch: 'master'
            }
        }
		stage('Build') {
			steps {
                sh 'mvn clean package'             
			}
        }
        
}
}
