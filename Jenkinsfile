pipeline {
agent any;
triggers {
    githubPush()
  }
stages {
stage('Code Quality') {
steps {
sh 'echo checking code quality'
git credentialsId: '17dabaa1-ee36-43ea-91a3-fe9e5de2e7b7', url: 'https://github.com/shazib96/Docker_App.git'
}
}
stage('Unit Tests') {
steps {
sh 'echo Testing the Applications'
}
}
stage('Build') {
steps {
sh 'echo Creating application Package'
}
}
stage('Delivery') {
steps {
sh 'echo Uploading the artifact to a repository'
}
}
stage('Deploy') {
steps {
sh 'echo Deploying the Application'
}
}
}
}
