pipeline {
    agent any
    stages {
        stage('Install') {
            steps {
                dir('Frontend') {
                    sh 'npm install'
                }
                
            }
        }
        stage('Test') {
            steps {
                dir('Frontend') {
                    sh 'ng test --progress false --watch false'
                }
                
            }
        }
    }
}
