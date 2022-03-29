// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    stages {
        stage('Main') {
            steps {
                sh """
                    echo ${BRANCH_NAME}
                    echo ${CHANGE_ID}
                """
            }
        }
    }
}
