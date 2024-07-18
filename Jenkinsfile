pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Build"){
            steps {
                echo("Hello Build")
            }
        }
        stage("Test"){
            steps {
                echo("Hello test")
                sh("Error")
            }
        }
        stage("Deploy"){
            steps {
                echo("Hello deploy")
            }
        }
    }
    post{
        always{
            echo "I always say hello again"
        }
        success{
            echo "build success"
        }
        failure{
            echo "Ob no fail"
        }
        cleanup{
            echo "dont care success of failure"
        }
    }
}