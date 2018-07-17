pipeline{
  agent any
  stages{
    stage('Deploy to staging'){
      steps{   
        sh "cd /var/jenkins_home/compose"
        sh "docker-compose up -d"
}
}
}
    post {
      always {
        sh "docker-compose down"
}
}
}
