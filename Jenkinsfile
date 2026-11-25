pipeline {
    agent any
    stages {
        stage('Checkout') { steps { echo 'Code pulled from GitHub' } }
        stage('Build')    { steps { sh 'echo Building...; ls -la' } }
        stage('Test')     { steps { sh 'echo Running tests...' } }
        stage('Deploy')   { steps { echo 'Deploy step' } }
    }
}
