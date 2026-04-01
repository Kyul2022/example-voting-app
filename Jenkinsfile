pipeline {

    agent any

    stages {
//nothing3
        stage("build") {
            steps{
                sh 'ls -l'
                sh 'cd example-voting-app'
                sh 'docker compose up -d'
            }
        }

        
        stage("test") {
            steps{
                sh 'ls -l'
                sh 'cd example-voting-app/result'
                sh 'docker compose -f docker-compose-test.yml up -d'
            }
        }

        
        stage("stage") {
            steps{
                echo "staging"
            }
        }

        
        stage("deploy") {
            steps{
                echo "deploying"
            }
        }


    }
}