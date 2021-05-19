pipeline {
    agent any

    tools {
        nodejs 'nodejs'
    }
    stages {

        stage('Build') {
            steps {
                nodejs('foonode') {
                    sh 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                nodejs('foonode') {
                    sh 'npm test'
                }
            }
        }
    }
}
