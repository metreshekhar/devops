pipeline{
    agent any
    stages{
        stage('Build') {
            steps {
                echo "Building ..."
            }
        } 
        
        stage('Prod') {
            steps {
                echo "production ..."
            }
        }

        stage('Dev') {
            steps {
                echo "Devopliment"
            }
        }
       
    }
}