pipeline {
    agent any
    
    environment {
        NAME = 'Nitin'
        CITY    = 'Datia'
    }
    
    tools {         
        maven 'Maven 3.3.9'  
        jdk 'JAVA_HOME'      
    }
    
    stages {
        stage("init") {
            steps {
                echo 'In side init !!'
                echo "Name =  ${NAME}"
                echo "City =  ${CITY}"
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
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
