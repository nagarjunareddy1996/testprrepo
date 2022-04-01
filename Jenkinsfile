// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    
    }
    stages {
        stage('checkout scm') {
            steps {
               
               sh """ 
                    eecho $env.BRANCH_NAME 
                    echo $env.GIT_BRANCH
                    echo $env.CHANGE_ID || true 
                    echo $env.CHANGE_BRANCH || true 
                    echo $env.CHANGE_URL
                    echo 'from feature branch'
                """
            }
        }
    }
}
