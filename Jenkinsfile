pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'This is dev environment'
      }
    }

    stage('QA') {
      steps {
        echo 'This is QA step'
        git 'https://github.com/LeafPages/Salesforce'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment requires manual approval'
        emailext(subject: 'TestMail', body: 'Testing purpose', to: 'passion.naren@gmail.com', attachLog: true)
      }
    }

  }
}