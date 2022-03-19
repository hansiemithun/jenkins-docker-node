pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' } 
    }

    stages {
        stage('init') {
            steps {
                echo "node version: "
                script {
                    sh 'node --version'
                    gv = load "script.groovy"
                }
            }
        }
    }
}
