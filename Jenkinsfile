pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t docker.io/madhanmohanreddyeeda/github-repo-user .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push docker.io/madhanmohanreddyeeda/github-repo-user'
      }
    }

  }
}