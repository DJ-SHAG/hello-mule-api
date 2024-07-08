pipeline {

	agent any
	
	stages {
		stage('Build') {
			steps {
				bat 'mvn -B -U -e -V clean -DskipTests package'
			
				  }
					    }
					    
		stage('Test') {
			steps {
				echo "************************* unit test execution **************************"
			
				  }
					    }
					    
					    
		stage('Deployment') {
			steps {
				bat 'mvn -U -V -e   -B  clean -DskipTests -Pdev deploy -DmuleDeploy' -X
			
				  }
					    }
	
	}




}
