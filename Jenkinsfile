pipeline{
    agent any

    tools{
        maven "3.6.0"
    }

    stages{
        stage("Build"){
            steps {
                bat  "mvnw.cmd -version"
                bat  "mvnw.cmd clean install"
            }
        }
    }

    post{
        always{
            cleanWs()
        }
    }
}