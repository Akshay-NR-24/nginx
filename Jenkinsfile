pipeline{
  agent none; 
  stages{
    stage('nginx'){
      agent { docker {image 'nginx'}}
      steps{
        sh '''
        nginx -v
        '''
      }
    }
    stage('Dockerfile'){
      agent { label 'Master' }
      steps{
        sh '''
               cd /home/ubuntu
                docker run -it -d --name container1 nginx
                '''
  }
}
  }
}
