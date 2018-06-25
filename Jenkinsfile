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
        stage('Test') {
            steps {
                withMaven(maven : 'MyMaven'){
                sh 'mvn test'
                }
            }
        }
        
    }
}
