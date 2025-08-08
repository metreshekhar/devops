pipeline{
    agent any
    stages{
        stage('Build & test') {
            stages{
                stage('Compile') {
                    steps {
                        echo "hello this is computing"
                    }
                }
                stage('Unit testing') {
                    steps {
                        echo "running unit tests..."
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo "deployed....."
            }
        }
    }
}