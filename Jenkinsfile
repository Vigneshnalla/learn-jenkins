pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        disableConcurrentBuilds()
    }
    parameters {
        choice(name: 'environment', choices: ['dev', 'prod'], description: 'Select environment')
    }
    stages {

        stage('Dev') {
            when {
                expression {
                    params.environment == 'dev'
                }
            }
            steps {
                sh 'echo Pre Build for Dev...'
            }
        }

        stage('Prod') {
            when {
                expression {
                    params.environment == 'prod'
                }
            }
            steps {
                sh 'echo Build for Prod...'
            }
        }

        stage('Post Build') {
            steps {
                sh 'echo Post Build ...'
            }
        }
    }
}
