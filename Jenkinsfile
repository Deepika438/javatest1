pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Code Quality') {
            steps {
                echo 'Quality'
            }
        }
        stage('Deploy to Dev') {
            steps {
                echo 'Dev'
            }
        }
        stage('Deploy to Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Deploy to UAT') {
            steps {
                echo 'UAT'
            }
        }
        stage('Deploy to PreProd') {
            steps {
                echo 'Preprod'
            }
        }
        stage('Prod Approval') {
            steps {
                Script{
                    if(env.BRANCH.NAME == "master"){
                    input('Proceed for Prod Deployment ?')}
                    }
                }
                
            }
            stage('Deploy to Prod') {
            steps {
                echo 'Prod'

        }
    }
}
}