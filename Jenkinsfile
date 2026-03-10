pipeline { 
  agent any
  stages {
    stage('checkout'){
      steps{
        git checkout main
        git 'https://github.com/Ambarish777/myfirstrepo.git'
      }
    } 
    stage('Publish'){
      steps{
        publishHTML([
          //default parameters
          allowMissing:true,
          alwaysLinkToLastBuild:false,
          keepAll:false,

          //these paramaters changes acc.
          reportDir:'.',                 // . is root directory
          reportFiles:'demo.html',       // name of html file
          reportName:'MY HTML PAGE'
        ])
      }
    }
  }
} 
