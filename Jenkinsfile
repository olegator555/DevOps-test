pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh "export PATH=/Users/Oleg/Downloads/apache-maven-3.8.5/bin:$PATH | mvn clean install"
                }
            }
        }
    }
    post {
        always {
            cleanWs()
        }
    }
}