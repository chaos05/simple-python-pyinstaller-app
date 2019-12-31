pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python3.8' 
                }
            }
            steps {
                sh 'python3.8 -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
