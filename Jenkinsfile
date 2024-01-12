pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=webappdevsecops -Dsonar.organization=webappdevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=39b178549b71cccd57ae0583a1a0ce4ca87a1872'
			}
        } 
  }
}
