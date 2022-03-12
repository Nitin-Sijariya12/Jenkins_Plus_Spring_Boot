pipeline {
    agent any
    
    environment {
        NAME = 'Nitin'
        CITY    = 'Datia'
    }
    
    tools {         
        maven 'maven_home'
        jdk 'java11'     
    }
    
    parameters {
            string(name: 'branchName', description: 'Please specify the branch name')
      }

    stages {    
        stage("init") {
            steps {  
                echo "Name =  ${NAME}"
                echo "City =  ${CITY}"
                echo "M2_HOME = ${M2_HOME}"
                echo "PATH = ${PATH}"
            }
        }
        stage("clean") {
            steps {
                 echo 'In side clean !!'
                 sh 'mvn clean' 
            }
        }
        stage(" test and build") {
            steps {
                echo 'In side build !!'
            }
        }
        stage("deploy") {
            steps {
                 echo 'In side deploy !! test branch !!'
            }
        }
    }   
}
