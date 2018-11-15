pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean"
            }
        }
        stage('--test--') {
            steps {
                sh "/opt/apache-maven-3.6.0/bin/mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "/opt/apache-maven-3.6.0/bin/mvn package"
            }
        }
    }
}
