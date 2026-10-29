
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Getting Java project from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Java project with Maven'
                bat 'mvn clean package'
            }
        }
    }
}
