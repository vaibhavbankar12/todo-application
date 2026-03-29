pipeline {
    agent any
    stages {
        stage ('Clone Repo') {
            steps {
                git url:'https://github.com/vaibhavbankar12/todo-application.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn clean package -dskipTests'
            }
        }
    }
}
