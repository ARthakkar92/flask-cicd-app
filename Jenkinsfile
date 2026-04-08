pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo "Installing dependencies..."
                sh 'python3 -m venv venv'
                sh '. venv/bin/activate && pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh '. venv/bin/activate && pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to staging..."
                sh 'nohup python3 app.py &'
            }
        }
    }
}
