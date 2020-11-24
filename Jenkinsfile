pipeline{
  agent{
    docker{
      image "node:8-alpine"
    }
  }
  stages{
    stage("Biuld"){
      steps{
        sh "cmod +x ./scripts/dropdb.sh"
        sh "npm install"
      }
    }
    stage("Test"){
      steps{
        sh "npm run test:ci"
      }
    }
  }
}
