pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                bat 'curl -X POST http://localhost:8081/'
            }
        }
    }
}
