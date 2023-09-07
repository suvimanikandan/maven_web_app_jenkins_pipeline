pipeline{
    agent any
    environment {
        PATH = "$PATH:apache-maven-3.9.4/bin"
    }
    stages{
       stage('GetCode'){
            steps{
				git branch: 'main',
                url: 'https://github.com/suvimanikandan/maven_web_app_jenkins_pipeline.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }       
    }
}
