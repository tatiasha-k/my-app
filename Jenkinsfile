pipeline {
    agent any 
    tools {
       maven 'default'
    }
    stages {
        stage('--- clean ---') { 
            steps {
                sh "mvn clean"

            }
        }
        stage('--- Test ---') { 
            steps {
                sh "mvn test " 
            }
        }
        stage('--- Deploy ---') { 
            steps {
                sh "mvn package " 
            }
        }
    }
}
