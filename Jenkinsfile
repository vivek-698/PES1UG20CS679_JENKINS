pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
              sh"g++ newfile.cpp -o outputfile"
              build job:"PES1UG20CS679-1"
      }
    }
    stage('Test'){
      steps{
              sh"./outputfile"
              
      }
    }
  }
  post{
    success{
      echo "pipeline completed"
    }
    failure{
echo "pipleline failed"
    }
  }
}
