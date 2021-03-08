pipeline {
    agent any
    stages{
        stage('Compile Stage 1') {
            steps {
                {
                    sh 'mvn clean compile'
                }
            }   
        }
    }
        stage('Testing Stage') {
            steps {
                withMaven(maven : 'my-maven') {
                    sh 'mvn test'
                }
            }
        }
        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'my-maven') {
                    sh 'mvn package'
                }
            }
        }
    }
}






