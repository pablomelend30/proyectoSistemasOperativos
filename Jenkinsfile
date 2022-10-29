pipeline {
    agent { docker { image 'node:16.17.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
        stage('Install Packages (Node.js)') {
            steps {
			    nodejs(
			        nodeJSInstallationName: 'nodejs10') {
			      sh "npm install"
			    }
            }
        }
    }
}