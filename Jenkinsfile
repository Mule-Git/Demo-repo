
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
                   pip install pytest
                   pip list
             '''
         }
      }
      stage('Test') {
         steps {
            echo '-----tested'
              sh ''' source Jenkins_venv_OS/bin/activate
                    pytest /Users/mule/Desktop/Learnings/Learning_Python/python_test_project/tests -v

                   
                '''
         }
      }
      stage('Deploy') {
         steps {
            echo '----Deployed'
         }
      }
   }
}

