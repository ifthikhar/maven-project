pipeline {
    agent any
	
    tools {
        maven 'localMaven'
    }
 
    stages{
        stage('Build'){
            steps {
                 C:\apache-maven-3.5.3\bin 'mvn clean package'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/*.war'
                }
            }
        }
    }
}
