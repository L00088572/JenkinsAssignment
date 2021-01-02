pipeline {
    agent any

    tools{
        maven 'maven3.6'
    }

    stages {

        // stage('Checkout') {
        //     steps {
        //         checkout([$class: 'GitSCM', branches: [[name: 'main']],
        //         doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], 
        //         userRemoteConfigs: [[url: 'https://github.com/L00088572/JenkinsAssignment.git']]]) 
        //    }
        // }

        stage('Build Code') {
            steps {
              bat 'mvn -f app/pom.xml clean install'
            }
        }

        stage('Run Tests') {
            steps {
              bat 'mvn -f app/pom.xml test'
            }
        }
    }
}