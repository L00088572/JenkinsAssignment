pipeline {
    agent any

    tools{
        maven 'maven3.6'
    }

    stages {

         stage ("Checkout") {
            git branch: 'main',
            url: 'https://github.com/L00088572/JenkinsAssignment.git'
        }

        stage('Test') {
            steps {
              echo 'Testing..'
            }
        }
    }
}