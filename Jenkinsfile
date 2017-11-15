pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        git(url: 'git@github.com:elenavnera/hello-world.git', branch: 'master', changelog: true, poll: true)
      }
    }
    stage('Pool Bamboo for deployment') {
      steps {
        build(job: 'Bamboo-poll', quietPeriod: 30, wait: true)
      }
    }
  }
}