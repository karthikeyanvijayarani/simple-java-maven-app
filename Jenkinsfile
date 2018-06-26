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
       
        stage('Testingh') {
            steps {
                withMaven(maven : 'MyMaven'){
                sh 'mvn test'
                }
            }
        }
        
    }
}
