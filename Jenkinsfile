pipeline {
    agent { label 'java' }
    stages {
        stage('Test') {
            agent {
                docker {
                    image 'openjdk:11.0.15-slim'
                }
            }
            steps {
                sh './gradlew clean build'
            }
        }
    }
}
