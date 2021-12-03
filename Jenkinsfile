pipeline {
    agent { 
        docker { 
            image 'golang:1.17.2'
        }
    }
    stages {
        stage('init') {
            steps {
                echo 'hello world'
                sh 'go env'   
            }
        }
        stage('build') {
            steps {
                echo 'build'
                sh 'pwd'
            }
        }
    }
}
