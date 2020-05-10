pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /home/GitHub/.m2:/root/.m2'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sh \'mvn -B -DskipTests clean package\''
      }
    }

  }
}