pipeline {
   agent { label 'slave4' }
    stages {
        stage('clone step') {
            steps { 
               sh 'rm -rf hello-world-war'
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
