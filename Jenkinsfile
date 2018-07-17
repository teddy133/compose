pipeline{
  agent any
  stages{
    stage('Deploy to staging'){
      sh "docker-compose up -d"
}
}
    post {
      always {
        sh "docker-compose down"
}
}
}
