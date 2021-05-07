pipeline {
   agent any

   stages {
      stage('Build') {
         steps {
            echo '------built'
            sh label: '', script: '/Users/mule/Desktop/Learnings/Learning_Python/python_test_project/py3_9_0/bin/python -m venv Jenkins_venv_OS'
            sh label: '', script: 'source Jenkins_venv_OS/bin/activate'
            sh label: '', script: '/Users/mule/Desktop/Learnings/Learning_Python/python_test_project/py3_9_0/bin/python -m venv Jenkins_venv_OS'
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




