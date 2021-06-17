pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                dir('Frontend') {sh 'npm install'}
                
            }
        }
        stage('Test') {
            steps {
                dir('Frontend') { sh 'ng test --progress false --watch false'}
                
            }
        }
        stage('Delivery') {
            steps {
                dir('Frontend') { sh 'npm run build'}
                
            }
        }
        stage('Deploy') {
            steps {
                dir('Frontend') { sh 'mv dist/Frontend/* /var/www/html'}
                
            }
        }
    }
}
