// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any

     
    stages {
        stage('Main') {
            def BRANCH_NAME = "$env.BRANCH_NAME"
            def branch_parts =  "${BRANCH_NAME}".tokenize('/')
            steps {
               sh """ 
                   /*
                    echo $env.BRANCH_NAME 
                    echo $env.GIT_BRANCH
                    echo $env.CHANGE_ID || true 
                    echo $env.CHANGE_BRANCH || true 
                    */
                    echo "$BRANCH_NAME"
                    echo "$branch_parts"
                    echo 'from feature branch'
                """
            }
        }
    }
}
