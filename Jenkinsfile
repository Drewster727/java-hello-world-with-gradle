pipeline {
     agent { label 'java' }
     stages {
         stage('Clean Workspace') {
             steps {
                  deleteDir()                  
             }
         }
         stage('Clone Project') {
             steps {                  
                  checkout scm                  
             }
         }
         stage('Build') {
             steps {                  
                  sh './gradlew clean build'
             }              
             post {
                 always {
                     sh 'echo done!'
                 }
             }
         }
     }
 }
