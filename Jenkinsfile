pipeline{
   stage('SCM Checkout'){
     git 'https://github.com/laith-leo/pipeline-demo.git'
   }
   stage('Compile-Package'){
      // Get maven home path
      //def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "mvn package"
   }
   stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'laith@laith.info'
   }
}
