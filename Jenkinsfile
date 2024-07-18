pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Hello"){
            steps {
                echo("Hello pipeline")
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