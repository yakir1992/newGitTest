pipeline {
  
  agent any
  
  stages {
    
            stage("test") {
      
      steps {
        script
        echo 'Testing the application...'
        echo 'Executing the pipeline for branch $BRANCH_NAME'
      }
      }
    
    stage("build") {
      when {
        expression{
          BRANCH_NAME == 'master'
        }
      }
      steps {
        echo 'building the application'
      }
      
    }
    
    }    
        stage("deploy") {
       when {
        expression{
          BRANCH_NAME == 'master'
        }
      }
      steps {
        echo 'deploying the application'
      }
      
    }
    
  }
  
}
