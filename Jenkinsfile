pipeline {
    agent none
    stages {
        stage('Run on Docker') {
            agent {
                docker {
                    image 'maven:3.9.2-eclipse-temurin-17-alpine'
                    label 'slave01'
                }
            }
            steps {
                checkout scm
                sh './push_to_docker.sh'
            }
        }
    }
}

