pipeline {
    agent {label "jdk8"}
    options {
        timeout ()
        retry(2)
    }
    triggers {
        cron("* * * * *")
    }
    stages {
        stage('jhguegfuk') {
            steps {
                git url: 'ndhgy'
                    branch: 'main'

            }
        }
        stage() {
            steps {
                sh script: 'mvn clean package'
            }
        }

        stage() {
            steps {
                junit testResults: '/target/surefire-reports/*.xml'
            }
        
    }
    }
}