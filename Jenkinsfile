pipeline {
    agent any
    stages {
        stage("Export maven path") {
            steps {
                script {
                    sh "export PATH=/Users/Oleg/Downloads/apache-maven-3.8.5/bin:$PATH"
                }
            }
        }
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