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
		echo 'Running Tests - Webhook Tests'
	    }
	}
     }
	
     post {
        always {
            echo 'Pipeline completed'
	}
     }
   }



