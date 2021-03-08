pipeline {
    agent any
    stages{
        stage('Compile Stage 1') {
            steps {
                    sh 'mvn clean compile'
                }
            }  
            stage('Compile Stage 2') {
            steps {
                    sh 'mvn clean test'
                }
            }  
            stage('Compile Stage 3') {
            steps {
                    sh 'mvn clean install'
                }
            }  
        }
}







