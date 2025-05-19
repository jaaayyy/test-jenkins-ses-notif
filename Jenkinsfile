pipeline {

  agent any
  
  stages{
    stage ('Build'){
      steps{
        echo "Builing the project"
        sh 'whoami && echo date'
    }
  }
  }
    post{
      success{
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jaycp.cloud@gmail.com'
      }
      failure{
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jaycp.cloud@gmail.com'
      }
    }
}
