pipeline {
    agent { 
        docker { 
            image 'golang:1.17.2'
        }
    }
    parameters {
        choice(name: 'test', choices: [1, 2, 3], description: '')   
    }
    stages {
        stage('init') {
            when {
                expression { params.test == 2 }   
            }
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
