pipeline {
  agent any
  tools { 
        maven 'RNDLabsMaven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=rndlabs-buggy-webapp -Dsonar.organization=rndlabs -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=ef2abdad515ff6484460eda8d9e17d4fa79629be'
			}
        } 
  }
}
