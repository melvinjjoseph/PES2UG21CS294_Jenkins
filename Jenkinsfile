pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        build 'PES2UG21CS294-1'
        sh 'g++ main.cpp -o output'
      }
    }
    stage('Test'){
      steps{
      sh './outp'
      }
      
    stage('Deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
}
}