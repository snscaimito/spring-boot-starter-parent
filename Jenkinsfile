node {
    checkout scm
    
    stage('Build') {
        docker.image('maven:3-jdk-11').inside('-v $HOME/.m2:/root/.m2') {
			sh "mvn package"
      	}
    }
}
