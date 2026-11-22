pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/nourane007/gestion-projets-backend.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
    }
}
