pipeline {

    agent any

    stages {
//nothing3
        stage("build") {
            steps{
                tree ./
                sh 'docker compose up -d'
            }
        }

        
        stage("test") {
            steps{
                sh 'cd ./result'
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