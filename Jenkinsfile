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
               sh 'sonar-scanner -Dsonar.host.url=http://172.31.80.223:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=user'
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