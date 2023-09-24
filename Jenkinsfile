pipeline {
    agent {
        node {
            label 'maven-slave'
        }
    }

enviroment = {
    PATH = "/opt/apache-maven-3.9.4/bin:$PATH"
}
stages {
   stage("Build"){
       steps {
          sh 'mvn clen deploy'
       }
   }
 }
}