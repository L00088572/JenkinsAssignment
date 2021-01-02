pipeline {
    agent any

    tools{
        maven 'maven3.6'
    }

    stages {
        stage('GIT Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: 'main']],
                doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], 
                userRemoteConfigs: [[url: 'https://github.com/L00088572/JenkinsAssignment.git']]]) 
           }
        }
        stage('Test') {
            steps {
              echo 'Testing..'
            }
        }
    }
}