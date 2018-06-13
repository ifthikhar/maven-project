pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                echo 'Now building...'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    
                }
            }
        }
    }
}
