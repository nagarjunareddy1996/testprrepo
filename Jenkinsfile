// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    environment {

     def branch_name = "$env.BRANCH_NAME"
     // def change_branch = "$env.CHANGE_BRANCH"
     def branch_parts =  "${branch_name.split("/") ?: env.CHANGE_BRANCH.split("/")}"
    }
    stages {
        stage('checkout scm') {
            steps {
               
               sh """ 
                    echo $branch_name
                    echo $branch_parts
                    echo 'from feature branch'
                """
            }
        }
    }
}
