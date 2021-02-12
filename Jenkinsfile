pipeline{
    agent any

    tools{
        maven "3.6.0"
    }

    stages{
        stage("Build"){
            steps {
                dir("sigo-ci-sample"){
                    bat  "mvnw.cmd -version"
                    bat  "mvnw.cmd clean install"
                }
               
                
            }
        }
    }

    post{
        always{
            cleanWs()
        }
    }
}