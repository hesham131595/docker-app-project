pipeline {
    agent any 
    stages {
        stage("build") {
            steps {
                checkout scmGit(branches: [[name: '*/dev']], extensions: [], userRemoteConfigs: [[credentialsId: 'app', url: 'https://github.com/hesham131595/docker-app-project.git']])
            }
        }

         stage("test") {
            steps {
                echo 'testing build'
            }
        }

         stage("deploy") {
            steps {
                echo 'deploying build'
            }
        }
    }
}
