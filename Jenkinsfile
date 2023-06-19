node('slave01'){

          checkout scm
          def main=docker.image('maven:3.9.2-eclipse-temurin-17-alpine')
          main.inside('-v /var/run/docker.sock:/var/run/docker.sock '){
          sh '''
             ./push_to_docker.sh
          '''
             }
