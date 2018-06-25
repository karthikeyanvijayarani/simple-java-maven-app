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
        stage('Deploy') {
            steps {
                withMaven(maven : 'MyMaven'){
                sh 'mvn deploy'
                }
            }
        }
    }
}
