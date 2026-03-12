pipeline {

agent any

stages {

stage('Clone Repository') {
steps {
git 'https://github.com/Aravindh-Cs/examdevops.git'
}
}

stage('deploy') {
steps {
bat 'http://localhost:8081/'
}
}
}
}
