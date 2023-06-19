node('slave01'){
          
	  checkout scm
	  def main=docker.image('maven:3.9.2-eclipse-temurin-17-alpine')
	  main.inside{
             ./push_to_docker.sh
	  }


}
