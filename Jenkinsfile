pipeline {
  agent {
    docker {
      image 'maven'
      args '-f objects-in/pom.xml  -DskipTests=true'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -f objects-in/pom.xml  -DskipTests=true'
      }
    }
  }
}