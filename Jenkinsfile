pipeline{
  agent{ docker { image 'nginx:latest' } }
  stages{
    stage('log version info'){
      steps{
        sh 'sudo apt update'
        sh 'sudo apt install nginx -y'
        sh 'nginx --version'
      }
    }
  }
}
