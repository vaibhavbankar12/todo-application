pipeline {
    agent any
    stages {
        stage ('Clone Repo') {
            steps {
                git credentialsId: 'githut-credentials' 
                url:'https://github.com/vaibhavbankar12/todo-application.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn clean package -DskipTests'
            }
        }
    }
}
