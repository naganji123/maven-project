node{
  stage('scm checkout'){
       git 'https://github.com/naganji123/maven-project'  
 }
  stage('compile-package'){
       //get maven home path
       def mvnHome = tool name: 'maven-3', type: 'maven'
       sh "${mvnHome}/bin/mvn package"
  }
  satge('email notification'){
       //email notification
       mail bcc: '', body: '''hi welcome to jenkins 
       email notification 
       alert
       thanks,
       naganji.k''', cc: '', from: '', replyTo: '', subject: 'jenkins job', to: 'nagan.msp@gmail.com'
  }
 }
  
