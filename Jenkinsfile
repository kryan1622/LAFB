pipeline{
	agent any
        stages{
		stage('---build---'){
                        steps{
                               sh "docker-compose build"
                        }
                }
		stage('---push---'){
   			withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'dockerhub', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']]) {
      			sh 'docker login -u "$USERNAME" -p "$PASSWORD"'
      			cont.push()
		}
		stage('---deploy---'){
			steps{
				sh "docker stack deploy --compose-file docker-compose.yaml devops"
			}
		}
	}
}
