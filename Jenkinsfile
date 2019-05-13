  node{
   stage('SCM Checkout'){
     git 'https://github.com/sivaom/my-app-1'
   }
   stage('Compile-Package'){
    
      def mvnHome =  tool name: 'Maven-3.6.1', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }
   stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Sri''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'samraj35@yahoo.com'
   }
 }


