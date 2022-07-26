pipeline{
  agent any

  stages{
    stage("Delete Old Container"){
      steps {
        catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
          echo "Delete the container"
        }
      }
    }
    stage("Building") {
      steps {
        echo "Building App"

        echo "Building FrontEnd"
      }
    }

    stage("Test"){
      steps{
        echo "Testing begin testing2"
      }
    }

    stage("Deploy"){
      steps{
        echo "deploy begin"
      }
    }
  }

  post {
    failure {
      echo "No!! it fail"
    }
    success {
      echo "Yes!! it work"
    }
  }
}
