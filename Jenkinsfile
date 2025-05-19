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
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jay@cloud-bridge.co.uk','jay.clemen@outlook.com'
      }
      failure{
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jay@cloud-bridge.co.uk','jay.clemen@outlook.com'
      }
    }
}
