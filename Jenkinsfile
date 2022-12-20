pipeline{
  agent { docker {image 'nginx:latest'}}
  stages{
    stage('nginx'){
      steps{
        sh '''
        nginx -v
        '''
      }
    }
  }
}
