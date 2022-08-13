pipeline{
    agent any
    stages{
    stage("Build"){
        steps{
            echo "Build"
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
    }
}