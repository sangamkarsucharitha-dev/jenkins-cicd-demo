pipeline {
    agent any

    stages {
        stage('Build') { 
            steps {
                echo 'Building application'
	    }
        }
        
        stage('Test') {
	    steps {
		echo 'Running Tests'
	    }
	}
     }
	
     post {
        always {
            echo 'Pipeline completed'
	}
     }
   }



