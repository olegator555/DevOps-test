pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    withMaven(maven: 'mvn') {
                        sh "mvn clean verify"
                    }
                }
            }
        }
    }
}