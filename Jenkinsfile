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
                cd /home/ubuntu
                docker run -it -d --name assigncontainer nginx
                '''
  }
}
  }
}
