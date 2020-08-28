pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
               // sh "rm -rf helloworld"
                //sh "git clone https://github.com/chandu-technologia/helloworld.git"
               sh "/usr/apache-maven-3.6.3/bin/mvn clean"
              // sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "/usr/apache-maven-3.6.3/bin/mvn test"
             //  sh "mvn test"
            }
        }
        stage('Package') { 
            steps {
               sh "/usr/apache-maven-3.6.3/bin/mvn package" 
              //sh "mvn package"
            }
        }
    }
}
