pipeline {
    agent {
        label 'AGENT-1'
    }
    stages {
        stage('Pre Build') {
            steps {
                sh 'echo Pre Build ...'
            }
        }
        stage('Build') {
            steps {
                 sh 'echo Build ...'
            }
        }
        stage('Post Build') {
            steps {
                 sh 'echo Post Build ...'
            }
        }
    }
}
