pipeline{
    agent any

    tools{
        maven "3.6.0"
    }

    stages{
        stage("Build"){
            steps {
                dir("sigo-ci-sample"){
                    sh  "mvn -version"
                    sh  "mvn clean install"
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