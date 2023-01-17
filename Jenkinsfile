pipeline {
    agent any
    stages {
        stage('Test python') {
            steps {
                sh "python -m pip install --upgrade pip"
                sh "if [ -f requirements.txt ]; then pip install -r requirements.txt; fi"
                echo 'Hello World'
                sh "python -m unittest"
            }
        }
    }
}
