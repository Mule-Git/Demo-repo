
pipeline {
    agent any


   stages {
      stage('Build') {
         steps {
            echo '------built'
            sh ''' /Library/Frameworks/Python.framework/Versions/3.9/bin/python3 -m venv Jenkins_venv_OS
                   source Jenkins_venv_OS/bin/activate
                   python --version
                   pip --version
                   pip list
             '''
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

