pipeline {

    agent { label 'linux' }

    triggers {
      githubPush()
    }

    stages {
        stage('Run Docker Compose App') {
            steps {
               sh "sudo docker-compose build"
               sh "sudo docker-compose up -d"
            }
        }
    }
}
