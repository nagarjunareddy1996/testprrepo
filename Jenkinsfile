// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    stages {
        stage('Main') {
            steps {
                echo BRANCH_NAME
                echo CHANGE_ID
                echo CHANGE_BRANCH  
                sh 'from feature branch'
            }
        }
    }
}
