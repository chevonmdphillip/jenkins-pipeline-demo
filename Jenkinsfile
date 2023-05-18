pipeline {
    tools {
        maven 'Maven-3.9.2'
    }
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn -version'
                sh 'mvn clean install'
        }
    }
}
    post {
        always {
            cleanWs()
        }
    }
}