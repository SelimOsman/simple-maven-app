pipeline {
    agent any 
    tools {
        maven "MAVEN"
        jdk "JDK9"
    }
    stages {
        stage('Compile') { 
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') { 
            steps {
                sh 'mvn package'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy stage'
            }
        }
        stage('Notification') { 
            steps {
                echo 'Notify STage'
            }
        }
    }
}
