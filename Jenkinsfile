pipeline {

agent any

stages {

stage('Clone Repository') {
steps {
git 'https://github.com/Aravindh-Cs/examdevops.git'
}
}

stage('Build Docker Image') {
steps {
bat 'docker build -t cicd-webapp .'
}
}

stage('Run Docker Container') {
steps {
bat '''
docker stop cicd-webapp
docker rm cicd-webapp
docker run -d -p 8082:80 --name cicd-webapp cicd-webapp
'''
}
}

}

}
