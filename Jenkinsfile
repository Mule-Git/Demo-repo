pipeline {
   agent any

   stages {
      stage('Build') {
         steps {
            echo '------built'
            sh label: '', script: '/Library/Frameworks/Python.framework/Versions/3.9/bin/python3 -m venv Jenkins_venv_OS'
            sh label: '', script: 'source Jenkins_venv_OS/bin/activate'
            sh label: '', script: 'python --version'
            sh label: '', script: 'pip --version'
            sh label: '', script: 'pip list'
         }
      }
      stage('Test') {
         steps {
            echo '-----tested'
         }
      }
      stage('Deploy') {
         steps {
            echo '----Deployed'
         }
      }
   }
}




