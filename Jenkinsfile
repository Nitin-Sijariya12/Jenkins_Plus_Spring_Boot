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
                echo "BRANCH_NAME :: $BRANCH_NAME"
                 echo "BRANCH_IS_PRIMARY :: $BRANCH_IS_PRIMARY"
                 echo "CHANGE_ID :: $CHANGE_ID"
                 echo "CHANGE_URL :: $CHANGE_URL"
                 echo "CHANGE_TITLE :: $CHANGE_TITLE"
                 echo "CHANGE_AUTHOR :: $CHANGE_AUTHOR"
                 echo "CHANGE_AUTHOR_DISPLAY_NAME :: $CHANGE_AUTHOR_DISPLAY_NAME"
                 echo "CHANGE_AUTHOR_EMAIL :: $CHANGE_AUTHOR_EMAIL"
                 echo "CHANGE_TARGET :: $CHANGE_TARGET"
                 echo "CHANGE_BRANCH :: $CHANGE_BRANCH"
                 echo "CHANGE_FORK :: $CHANGE_FORK"
                 echo "TAG_NAME :: $TAG_NAME"
                 echo "TAG_TIMESTAMP :: $TAG_TIMESTAMP"
                 echo "TAG_UNIXTIME :: $TAG_UNIXTIME"
                 echo "TAG_DATE :: $TAG_DATE"
                echo "JOB_DISPLAY_URL :: $JOB_DISPLAY_URL"
                echo "RUN_ARTIFACTS_DISPLAY_URL :: $RUN_ARTIFACTS_DISPLAY_URL"
                echo "RUN_CHANGES_DISPLAY_URL :: $RUN_CHANGES_DISPLAY_URL"
                echo "RUN_TESTS_DISPLAY_URL :: $RUN_TESTS_DISPLAY_URL"
                echo "CI :: $CI"
                echo "BUILD_ID :: $BUILD_ID "
                echo "JOB_NAME :: $JOB_NAME"
                echo "JOB_BASE_NAME :: $JOB_BASE_NAME"
                echo "BUILD_TAG :: $BUILD_TAG"
                echo "EXECUTOR_NUMBER :: $EXECUTOR_NUMBER"
                echo "NODE_NAME :: $NODE_NAME"
                echo "NODE_LABELS :: $NODE_LABELS"
                echo "WORKSPACE :: $WORKSPACE"
                echo "WORKSPACE_TMP :: $WORKSPACE_TMP"
                echo "JENKINS_HOME :: $JENKINS_HOME"
                echo "JENKINS_URL :: $JENKINS_URL"
                echo "BUILD_URL :: $BUILD_URL"
                echo "JOB_URL :: $JOB_URL"
                echo "GIT_COMMIT :: $GIT_COMMIT"
                echo "GIT_PREVIOUS_COMMIT :: $GIT_PREVIOUS_COMMIT"
                echo "GIT_PREVIOUS_SUCCESSFUL_COMMIT :: $GIT_PREVIOUS_SUCCESSFUL_COMMIT"
                echo "GIT_BRANCH :: $GIT_BRANCH"
                echo "GIT_LOCAL_BRANCH :: $GIT_LOCAL_BRANCH"
                echo "GIT_CHECKOUT_DIR :: $GIT_CHECKOUT_DIR"
                echo "GIT_URL :: $GIT_URL"
                echo "GIT_COMMITTER_NAME :: $GIT_COMMITTER_NAME"
                echo "GIT_AUTHOR_NAME :: $GIT_AUTHOR_NAME"
                echo "GIT_COMMITTER_EMAIL :: $GIT_COMMITTER_EMAIL"
                echo "GIT_AUTHOR_EMAIL :: $GIT_AUTHOR_EMAIL"
                
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
