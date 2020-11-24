pipeline{
  agent{
    docker{
      image "node:8-alpine"
    }
  }
  stages{
    stage("Biuld"){
      steps{
        sh "npm install"
      }
    }
  }
}
