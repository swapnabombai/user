pipeline {
    agent {
      node { label 'practice' }

    }

    stages {

        stage('build') {
            steps {
                 sh 'npm install'
                 // sh 'npm test'
            }
        }

        stage('Unit tests') {
           steps {
                echo 'unit tests'
                // sh 'mvn test'
           }
        }

        stage('Code Analysis') {
           steps {
               echo 'Code Analysis'
           }
        }

        stage('Security Scans') {
           steps {
               echo 'Security Scans'
           }
        }

        stage('Publish a Artifact') {
           steps {
               echo 'Publish a Artifact'
           }
        }
    }
}