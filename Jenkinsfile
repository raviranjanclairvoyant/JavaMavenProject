pipeline {
    agent any
      tools {
        maven 'maven-3.6.3'
      }

    stages {
        stage('New Build') {
            steps {
              sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                gcloud --help
                echo 'Deploying....'
            }
        }
    }
}