pipeline {
    agent any
    stages {
        stage('Test python') {
            steps {
                python -m pip install --upgrade pip
                if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
                echo 'Hello World'
                python -m unittest
            }
        }
    }
}
