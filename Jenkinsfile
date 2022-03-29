// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    stages {
        stage('Main') {
            steps {
               sh """ 
                    echo $env.BRANCH_NAME 
                    echo $env.CHANGE_ID || true 
                    echo $env.CHANGE_BRANCH || true 
                    echo 'from feature branch'
                """
            }
        }
    }
}
