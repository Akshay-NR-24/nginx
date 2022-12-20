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
    stage('Dockerfile'){
      steps{
        sh '''
               cd /home/ubuntu/workspace1
                docker run -it -d --name assigncontainer nginx
                '''
  }
}
  }
}
