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
        stage("clean") {
            steps {
                 echo 'In side clean !!'
                 sh 'mvn clean' 
            }
        }
        stage("build") {
            steps {
                echo 'In side build !!'
                sh 'mvn install' 
            }
        }
        stage("deploy") {
            steps {
                 echo 'In side deploy !!'
            }
        }
    }   
}
