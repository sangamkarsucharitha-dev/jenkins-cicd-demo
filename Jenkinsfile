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
		echo 'Running Tests - Webhook Test'
	    }
	}
     }
	
     post {
        always {
            echo 'Pipeline completed'
	}
     }
   }



