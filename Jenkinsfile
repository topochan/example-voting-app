node {
  stage "Checkout"
  checkout scm

  stage "Build"
  sh "docker-compose -f docker-compose.yml build"
}
