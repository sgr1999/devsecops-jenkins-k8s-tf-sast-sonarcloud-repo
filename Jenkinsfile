pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=sagarbuggywebapp -Dsonar.organization=CompileandRunSonarAnalysis
 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=09129aa98e7149d95484123d3997c3ad8f72780b'
			}
        } 
  }
}
