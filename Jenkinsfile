pipeline {
    agent any
    
    enviroment{
        Name = 'Nitin'   
    }
    
    stages {
        stage("init") {
            steps {
                echo 'In side init !!'
                echo "Name = ${Name}"
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
