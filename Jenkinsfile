pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                // This assumes a Windows agent and a URL endpoint
                bat 'curl -X POST http://localhost:8081/'
            }
        }
    }
}
