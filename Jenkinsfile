pipeline {
    agent { label 'java' }
    stages {
        stage('Test') {
            agent {
                label 'java'
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
