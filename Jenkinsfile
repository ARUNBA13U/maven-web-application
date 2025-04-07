pipeline{
    agent{ label "jenkins_slave" }
    tools {
        maven 'maven_3.9'
    }

    stages{
       stage('Code Checkout') {
        steps {
                            git 'https://github.com/ARUNBA13U/maven-web-application.git'
            }  
        }
       stage('Build'){
        steps{
            sh 'mvn clean install'
        }
       }

    }

