pipeline{
    //agent any
    //agent { docker { image 'maven:3.8.6-jdk-11' }}
    agent{ docker{image 'node:13.8'}}
    stages{
    stage("Build"){
        steps{
            echo "Build"
            sh "node --version"
        }
    }
    stage("Test"){
        steps{
            echo "Testing"
        }
    }
    stage("Inetgration stage"){
        steps{
            echo " New stage"
        }
    }
    }

    post{
        always{
            echo " I run always"
        }
        success{
            echo " I run success"
        }
        failure{
            echo " I run failure"
        }
        // other type of posts are "changed" and "unstable"
    }
}