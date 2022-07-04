pipeline {
   agent any
    stages {
        stage('clone step') {
            steps {
                sh 'git clone https://github.com/akshaygHX711/hello-world-war.git'
            }
        }
  stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
