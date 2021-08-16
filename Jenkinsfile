pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
		bat """pip3 install -r requirements.txt
		      python setup.py build"""
            }
        }
      //  stage('Test') {
        //    steps {
          //      echo 'Testing...'
		//bat 'pytest tests'
            //}
        //}
        stage('Deploy') {
            steps {
               bat 'python src/my_app.py'
            }
        }
    }
}
