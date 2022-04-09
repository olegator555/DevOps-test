pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    withMaven(maven: 'mvn') {
                        sh "export PATH=/Users/Oleg/Downloads/apache-maven-3.8.5/bin:$PATH"
                        sh "mvn clean verify"
                    }
                }
            }
        }
    }
}