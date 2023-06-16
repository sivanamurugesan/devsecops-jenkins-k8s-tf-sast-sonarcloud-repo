pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cherryorg -Dsonar.organization=cherryorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7905b912524bc54d9e23b0b78664c99cef663545'
			}
        } 
  }
}
