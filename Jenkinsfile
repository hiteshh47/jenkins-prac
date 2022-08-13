pipeline{
    //agent any
    agent { docker { image "maven-3.6.3" }}
    stages{
    stage("Build"){
        steps{
            echo "Build"
            sh "mvn --version"
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