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
stage('Use Credential') {
    steps {
	withCredentials([string(credentialsId: 'demo-secret', variable: 'MY_SECRET')]) {
    		sh 'some-command --token "$MY_SECRET"'
}
    }
}
     }
	
     post {
        always {
            echo 'Pipeline completed'
	}
     }
   }



