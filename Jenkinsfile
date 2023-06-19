node{
          
	  checkout scm
	  def main=docker.image('maven:3.9.2-eclipse-temurin-17-alpine').label('slave01')
	  main.inside{
	  sh '''
             ./push_to_docker.sh
          '''
	     }


}
