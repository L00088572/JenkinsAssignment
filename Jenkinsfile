pipeline {
    agent any

    tools{
        maven 'maven3.6'
    }

    stages {

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


