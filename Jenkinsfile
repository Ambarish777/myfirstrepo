pipeline{
  agent any
  stages{
    stage('checkout'){
      step{
        git 'https://github.com/Ambarish777/myfirstrepo.git'
      }
    } 
    stage('Publish'){
      steps{
        publishHTML([
          //default parameters
          allowMissing:true,
          alwaysLinktoLastBuild:false,
          keepAll:false,


          //these paramaters changes acc.
          reportDir:'.',                 // . is root directory
          reportFiles:'demo.html',       // name of html file
          reportName:'MY HTML PIPE PAGE'
        ])
          
        
      }
    }
    
  }
}
