pipeline {
    agent any

    stages {
        stage('build') {
            steps {
	       sh 'docker build -t python2/app .'
   	       sh 'docker images' 
            }
    
        }
    }
}

