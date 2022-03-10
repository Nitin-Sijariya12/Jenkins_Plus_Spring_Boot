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
    
    stages {
        stage("init") {
            steps {
                echo 'In side init !!'
                echo "BUILD_NUMBER :: $BUILD_NUMBER"
                echo "Name =  ${NAME}"
                echo "City =  ${CITY}"
                echo "M2_HOME = ${M2_HOME}"
                echo "PATH = ${PATH}"
            }
        }
        stage("build") {
            steps {
                 echo 'In side build !!'
                 sh 'mvn -Dmaven.test.failure.ignore=true clean install' 
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
