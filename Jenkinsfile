pipeline{
  agent any
  stages{
    stage("Checkout"){
      when{
        branch 'develop'
      }
     steps{
      git url:"https://github.com/javahometech/my-app-25", branch:"main"
     }
    }
    stage("Build"){
      when{
        branch 'develop'
      }
     steps{
      echo "Building app"
     }
    }
    stage("Dev Deploy"){
      when{
        branch 'develop'
      }
     steps{
      echo "Deploying to dev...."
     }
    }
    stage("Prod Deploy"){
      when{
        branch 'develop'
      }
     steps{
      echo "Deploying to prod...."
     }
    }
  }
}
