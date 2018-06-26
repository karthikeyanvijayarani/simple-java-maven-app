pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'MyMaven'){
                sh 'mvn clean compile'
                }
            }
        }
       
        stage('Testing ') {
            steps {
                withMaven(maven : 'MyMaven'){
                sh 'mvn test'
                }
            }
        }
        
    }
}
