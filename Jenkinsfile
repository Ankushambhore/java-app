pipeline {
    agent any

    triggers {
        githubPush() // This listens for GitHub webhook events
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Ankushambhore/java-app.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building automatically on commit...'
            }
        }
    }
}
