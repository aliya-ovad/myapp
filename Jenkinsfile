pipeline {
    agent any

    stages {
        stage('build') {
            steps {
             
	       sh 'docker build -t python2/app .'
   	       sh 'docker images' 
            }
    
        }
        stage('push') {
            steps {
        sh 'aws ecr get-login-password --region eu-central-1 | docker login --username AWS --password-stdin 040500316512.dkr.ecr.eu-central-1.amazonaws.com '
        sh 'docker tag  python2/app 040500316512.dkr.ecr.eu-central-1.amazonaws.com/python_app:2'
        sh '040500316512.dkr.ecr.eu-central-1.amazonaws.com/python_app:2'
            }

        }

    }
}

