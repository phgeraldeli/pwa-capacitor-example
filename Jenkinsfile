timestamps{
    node('node-js'){
        
        stage('Checkout'){
            checkout scm
        }
        
        stage('Install Dependencies'){
            sh 'npm install'
        }
        stage('Test'){
            sh 'npm test'
        }

        stage('Release'){
            sh 'npm run build-apk'
        }
    }
}