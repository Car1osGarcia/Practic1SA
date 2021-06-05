ipeline {
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
                    sh 'npm run test --watch=false'
                }
                
            }
        }
    }
}
