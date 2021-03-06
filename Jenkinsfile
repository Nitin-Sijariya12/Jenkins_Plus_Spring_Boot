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
                echo 'In side init !!'
                echo "BRANCH_NAME :: $env.BRANCH_NAME"
                echo "BRANCH_IS_PRIMARY :: $env.BRANCH_IS_PRIMARY"
                echo "CHANGE_ID :: $env.CHANGE_ID"
                echo "CHANGE_URL :: $env.CHANGE_URL"
                echo "CHANGE_TITLE :: $env.CHANGE_TITLE"
                echo "CHANGE_AUTHOR :: $env.CHANGE_AUTHOR"
                echo "CHANGE_AUTHOR_DISPLAY_NAME :: $env.CHANGE_AUTHOR_DISPLAY_NAME"
                echo "CHANGE_AUTHOR_EMAIL :: $env.CHANGE_AUTHOR_EMAIL"
                echo "CHANGE_TARGET :: $env.CHANGE_TARGET"
                echo "CHANGE_BRANCH :: $env.CHANGE_BRANCH"
                echo "CHANGE_FORK :: $env.CHANGE_FORK"
                echo "TAG_NAME :: $env.TAG_NAME"
                echo "TAG_TIMESTAMP :: $env.TAG_TIMESTAMP"
                echo "TAG_UNIXTIME :: $env.TAG_UNIXTIME"
                echo "TAG_DATE :: $env.TAG_DATE"
                echo "JOB_DISPLAY_URL :: $env.JOB_DISPLAY_URL"
                echo "RUN_ARTIFACTS_DISPLAY_URL :: $env.RUN_ARTIFACTS_DISPLAY_URL"
                echo "RUN_CHANGES_DISPLAY_URL :: $env.RUN_CHANGES_DISPLAY_URL"
                echo "RUN_TESTS_DISPLAY_URL :: $env.RUN_TESTS_DISPLAY_URL"
                echo "CI :: $env.CI"
                echo "BUILD_ID :: $env.BUILD_ID "
                echo "JOB_NAME :: $env.JOB_NAME"
                echo "JOB_BASE_NAME :: $env.JOB_BASE_NAME"
                echo "BUILD_TAG :: $env.BUILD_TAG"
                echo "EXECUTOR_NUMBER :: $env.EXECUTOR_NUMBER"
                echo "NODE_NAME :: $env.NODE_NAME"
                echo "NODE_LABELS :: $env.NODE_LABELS"
                echo "WORKSPACE :: $env.WORKSPACE"
                echo "WORKSPACE_TMP :: $env.WORKSPACE_TMP"
                echo "JENKINS_HOME :: $env.JENKINS_HOME"
                echo "JENKINS_URL :: $env.JENKINS_URL"
                echo "BUILD_URL :: $env.BUILD_URL"
                echo "JOB_URL :: $env.JOB_URL"
                echo "GIT_COMMIT :: $env.GIT_COMMIT"
                echo "GIT_PREVIOUS_COMMIT :: $env.GIT_PREVIOUS_COMMIT"
                echo "GIT_PREVIOUS_SUCCESSFUL_COMMIT :: $env.GIT_PREVIOUS_SUCCESSFUL_COMMIT"
                echo "GIT_BRANCH :: $env.GIT_BRANCH"
                echo "GIT_LOCAL_BRANCH :: $env.GIT_LOCAL_BRANCH"
                echo "GIT_CHECKOUT_DIR :: $env.GIT_CHECKOUT_DIR"
                echo "GIT_URL :: $env.GIT_URL"
                echo "GIT_COMMITTER_NAME :: $env.GIT_COMMITTER_NAME"
                echo "GIT_AUTHOR_NAME :: $env.GIT_AUTHOR_NAME"
                echo "GIT_COMMITTER_EMAIL :: $env.GIT_COMMITTER_EMAIL"
                echo "GIT_AUTHOR_EMAIL :: $env.GIT_AUTHOR_EMAIL"
                
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
                sh 'mvn test install' 
            }
        }
        stage("deploy") {
            steps {
                 echo 'In side deploy !! master branch'
            }
        }
    }   
}
