pipeline {
    agent any
    
    stages {
        stage("init") {
            steps {
                echo 'In side init !!'
                echo "Branch name = ${BRANCH_NAME}"
            }
        }
        stage("build") {
            steps {
                 echo 'In side build !!'
            }
        }
        stage("test") {
            steps {
                echo 'In side test'
            }
        }
        stage("deploy") {
            steps {
                 echo 'In side deploy'
            }
        }
    }   
}
