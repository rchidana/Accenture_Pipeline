pipeline {
  agent any
  stages {
    stage('Git Check Out') {
      steps {
        git(url: 'https://github.com/rchidana/Accenture_Pipeline.git', branch: 'master')
        echo 'Successfully Checkout from GitHub'
      }
    }

    stage('Compile') {
      steps {
        bat 'Compile.bat'
        echo 'Compiled Successfully!!'
      }
    }

    stage('Package') {
      steps {
        bat 'Package.bat'
        echo 'Packaged Successfully!!'
      }
    }

    stage('Deploy') {
      steps {
        bat 'Deploy.bat'
        echo 'Deployed!!'
        echo 'Super Easy to Use the BlueOcean UI for Pipeline Creation!!'
      }
    }

  }
}