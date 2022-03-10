pipeline {
    agent any
    
    environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE    = 'sqlite'
    }
    
    stages {
        stage("init") {
            steps {
                echo 'In side init !!'
                echo "Database engine is ${DB_ENGINE}"
                echo "DISABLE_AUTH is ${DISABLE_AUTH}"
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
