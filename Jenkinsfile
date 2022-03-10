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
                echo "BUILD_NUMBER" :: $BUILD_NUMBER
                echo "BUILD_ID" :: $BUILD_ID
                echo "BUILD_DISPLAY_NAME" :: $BUILD_DISPLAY_NAME
                echo "JOB_NAME" :: $JOB_NAME
                echo "JOB_BASE_NAME" :: $JOB_BASE_NAME
                echo "BUILD_TAG" :: $BUILD_TAG
                echo "EXECUTOR_NUMBER" :: $EXECUTOR_NUMBER
                echo "NODE_NAME" :: $NODE_NAME
                echo "NODE_LABELS" :: $NODE_LABELS
                echo "WORKSPACE" :: $WORKSPACE
                echo "JENKINS_HOME" :: $JENKINS_HOME
                echo "JENKINS_URL" :: $JENKINS_URL
                echo "BUILD_URL" ::$BUILD_URL
                echo "JOB_URL" :: $JOB_URL
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
