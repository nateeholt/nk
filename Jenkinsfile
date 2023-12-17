pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=natee-securityguru -Dsonar.organization=natee-securityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=01d5bd0d87d0047d7d25a4e7a12ae5b42c09ed38'
			}
    }		
  }
}
