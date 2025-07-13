pipeline {
    agent any
    stages {
        stage("Install Python") {
            steps {
                sh '''
                    sudo apt-get update
                    sudo apt-get install -y python3
                '''
            }
        }
        stage("Check Python Version") {
            steps {
                sh "python3 --version"
            }
        }
        stage("Running the application") {
            steps {
                sh "python3 hello_world.py"
            }
        }
    }
}
