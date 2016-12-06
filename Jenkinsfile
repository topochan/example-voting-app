node {
  stage "Checkout" {
    checkout scm
  }

  stage "Build" {
    sh "docker build -t topochan/vote ./vote"
    sh "docker build -t topochan/worker ./worker"
    sh "docker build -t topochan/result ./result"
  }

  stage "Push" {
    sh "docker push topochan/vote"
    sh "docker push topochan/worker"
    sh "docker push topochan/result"
  }


}
