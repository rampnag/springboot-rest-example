pipeline {
 agent any
stages {
  stage('CodeCheckOut') {
    steps {
      script {
       checkout scm
       /*def mvnHome = tool 'maven-3'
       def javaHome = tool 'JAVA_1.8'*/  
       }
      }
     }      
      stage('Build customer app code'){
        steps {
        script {
       sh 'sudo yum -y install unzip java-1.8.0-openjdk'
       sh 'sudo yum -y install maven'
         /* try{
          sh "mvn clean install"
           currentBuild.result = 'SUCCESS'
          } catch(Exception err){
          currentBuild.result = 'FAILURE'
         }*/
       }
      }
     }
    }
}
