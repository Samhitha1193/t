pipeline {
    agent any 
    stages {
        stage('Build'){
            steps{
                command 'mvn clean package'
                command "docker build . -t test:${env.BUILD_ID}"
            }
        }
    }
}
