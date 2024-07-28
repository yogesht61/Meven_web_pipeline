pipeline{
		agent any
		environment {
		PATH = "$PATH:/opt/apache-maven-3.9.8/bin"
	}
			stages{
				stage('GetCode'){
					steps{

					git branch: 'main',
						url: 'https://github.com/yogesht61/Meven_web_pipeline.git'

					}
				}
				stage('Build'){
						steps{
						sh 'mvn clean package'
					}
				}
			}	
	}		
