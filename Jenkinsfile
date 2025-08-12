pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test & Analyze') {
            parallel {
                stage('Unit Tests') {
                    steps {
                        echo 'Executing unit tests...'
                    }
                }
                stage('Integration Tests') {
                    steps {
                        echo 'Executing integration tests...'
                    }
                }
                stage('Static Analysis') {
                    steps {
                        echo 'Running code linter...'
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
