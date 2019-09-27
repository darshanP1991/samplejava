pipeline {
    agent any
    
    stages {
        
        stage ('Clone') {
            steps {
                git branch: 'master', url: "https://github.com/darshanP1991/samplejava"
            }
        }
        stage('Build') { 
            steps {
                bat 'mvn clean package' 
            }
        }
	}
}
