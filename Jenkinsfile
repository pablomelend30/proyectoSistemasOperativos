pipeline{
    agent {label 'main'}
    
    
    stages{
        stage('install'){
            steps{
                dir("build_node"){
                    sh "npm install"
                }
            }
        }
        stage('Test'){
            steps {
                dir("build_node"){
                    sh "npm test"
                }
            }
        }
        stage ('docer Build'){
            steps {
                echo "build"
            }
        }

        stage ('docker push'){
            steps{
                echo "push"
            }
        }
    }
    
}