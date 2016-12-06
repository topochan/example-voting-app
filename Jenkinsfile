node {
  stage "Checkout"
  checkout scm

  stage "Build"
  sh "docker build -t topochan/vote ./vote"
  sh "docker build -t topochan/worker ./worker"
  sh "docker build -t topochan/result ./result"
}
