pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp1975 -Dsonar.organization=asgbuggywebapp1975 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=bf827dbeda9716915d4cce3ae33505ba4e2c1f74'
			}
        } 
  }
}
