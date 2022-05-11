pipeline {
    agent {
        docker { image 'openjdk:11.0.15-slim' }
    }
    stages {
        stage('Test') {
            steps {
                sh './gradlew clean build'
            }
        }
    }
}
