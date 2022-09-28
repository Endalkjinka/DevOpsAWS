pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building Phase of CICD"
            }
        }
        stage('Test') {
            steps {
                echo "Testing Phase of CICD"
            }
        }
       stage('cat README') {
            when {
                branch "film-*"
           }
           steps {
             sh '''
               cat README.md
               '''
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying Phase of CICD"
            }
        }
    }
}
