pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    
    stages {
        
        stage ('Clone') {
            steps {
                git branch: 'master', url: "https://github.com/darshanP1991/samplejava"
            }
        
        stage('Build') { 
            steps {
                sh 'mvn clean package' 
            }
        }
}        
