pipeline {
  agent {
    dockerfile {
      filename 'jenkinsfile'
    }

  }
  stages {
    stage('') {
      steps {
        sh 'docker run -it -v maven-repo:/root/.m2 maven mvn archetype:generate # will reuse downloaded artifacts'
      }
    }
  }
  environment {
    jenkinsfile = 'jenkins'
  }
}