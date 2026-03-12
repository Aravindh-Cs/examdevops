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
bat 'docker run -d -p 8081:80 --name cicd-webapp cicd-webapp'
}
}

}
