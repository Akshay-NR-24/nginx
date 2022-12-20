pipeline{
  agent { docker {image 'nginx'}}
  stages{
    stage('nginx'){
      steps{
        sh '''
        nginx -v
        build run -it -d 3964ce7b8458
        '''
      }
    }
  }
}
