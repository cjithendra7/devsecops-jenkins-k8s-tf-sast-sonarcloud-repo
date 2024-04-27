pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mytestwebapp -Dsonar.organization=mytestwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a214c3553e4c689948eaac2d203ef548ddf7f577'
			}
        } 
  }
}
