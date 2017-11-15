pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        git(url: 'git@github.com:elenavnera/hello-world.git', branch: 'master', changelog: true, poll: true)
      }
    }
  }
}