// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent any
    environment {

     def branch_name = "$env.BRANCH_NAME"
     def branch_parts =  "${branchname.split("/") ?: 'env.CHANGE_BRANCH'}"
    }
    stages {
        stage('Main') {
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
