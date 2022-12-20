pipeline{
  agent { docker {image 'nginx'}}
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
