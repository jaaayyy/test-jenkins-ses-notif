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
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jr.cabido@cloud-bridge.co.uk'
      }
      failure{
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jr.cabido@cloud-bridge.co.uk'
      }
    }
}
