pipeline {

    agent any

    triggers {
      githubPush()
    }

    stages {
        stage('Run Docker Compose App') {
            steps {
               sh "docker-compose build"
               sh "docker-compose up -d"
            }
        }
    }
}
