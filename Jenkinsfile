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
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jay@cloud-bridge.co.uk'
      }
      failure{
        #emailext attachLog: true, body: 'Email sent out from Jenkins', subject: '$PROJECT_NAME - Build # $BUILD_NUMBER - $BUILD_STATUS!', to: 'rs.ranjitswain@gmail.com'
        emailext body: 'test email notification Jenkins', subject: 'test email notification Jenkins', to: 'jay@cloud-bridge.co.uk'
      }
    }
}
