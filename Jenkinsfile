pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Source code checkout successful'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Java application'
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Running JUnit test cases'
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging application'
                bat 'mvn package -DskipTests'
            }
        }
    }

    post {
        success {
            echo 'BUILD SUCCESSFUL'
        }

        failure {
            echo 'BUILD FAILED'
        }
    }
}
