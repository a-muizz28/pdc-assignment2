pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps { echo 'Code pulled from GitHub' }
        }
        stage('Build') {
            steps { sh 'python3 -m py_compile app.py test_app.py' }
        }
        stage('Test') {
            steps { sh 'python3 -m unittest -v test_app.py' }
        }
        stage('Run') {
            steps { sh 'python3 app.py' }
        }
    }
}
