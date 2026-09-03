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
        withCredentials([usernamePassword(credentialsId: 'secret', usernameVariable: 'MY_USER', passwordVariable: 'MY_SECRET')]) {
            sh 'echo "Credential is for pipeline"'
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



