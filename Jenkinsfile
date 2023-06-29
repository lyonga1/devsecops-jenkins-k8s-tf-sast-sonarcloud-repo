pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp-lyonga -Dsonar.organization=asgbuggywebapp-lyonga -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1385d50ebb0597783b4f8963e4b9ea743a2f6d5b'
			}
        } 
  }
}
