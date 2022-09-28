pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                sh 'echo stage1'
            }
        }
        stage('learning') {
            steps {
                git url: 'https://github.com/srikanthreddygajjala070/js-e2e-express-server.git', 
                    branch: 'main'
            }
        }
        stage('build') {
            steps {
            sh 'npm install'
            sh 'npm run build'
            }
        }
    }
}