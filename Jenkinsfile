pipeline {
    agent any
    stages{
    stage ('clone step')
    {
    steps{ 
        sh 'rm -rf hello-world-war'
        sh 'git clone https://github.com/akshaygHX711/hello-world-war.git' 
    }}
        
            stage ('maven build')
        {
            steps{
                sh 'mvn package'
            }}
            stage ('deploy')
        {
            steps
            {    
                sh 'sudo cp /home/slave4/workspace/hello_world/target/hello-world-war-1.0.0.war /home/slave4/workspace/hello_world/target/hello-world-war-pipeslave4.war
                sh 'sudo cp /home/slave4/workspace/hello_world/target/hello-world-war-pipeslave4.war /opt/apache-tomcat-9.0.64/webapps/'
            }}
            }
        }
    }
}
