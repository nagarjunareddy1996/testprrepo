// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any

     def branch_name = env.BRANCH_NAME
     def branch_parts =  "${branch_name}".split("/")
    stages {
        stage('Main') {
            steps {
               sh """ 
                   /*
                    echo $env.BRANCH_NAME 
                    echo $env.GIT_BRANCH
                    echo $env.CHANGE_ID || true 
                    echo $env.CHANGE_BRANCH || true 
                    */
                    echo $branch_name
                    echo $branch_parts
                    echo 'from feature branch'
                """
            }
        }
    }
}
