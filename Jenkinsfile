pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=madhurichakkawebapp -Dsonar.organization=Madhuri chakka -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=779d89528ba51fcfe805dd0e0195c5f362b8f5fb'
			}
        } 
  }
}
