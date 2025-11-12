pipeline {
    agent any

    triggers {
        githubPush()  // Responds to GitHub webhook
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Ankushambhore/java-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'javac welcome.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java welcome'
            }
        }
    }
}
