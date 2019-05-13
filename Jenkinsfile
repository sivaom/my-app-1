  node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app-1'
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
 //  stage('Slack Notification'){
       slackSend baseUrl: 'https://hooks.slack.com/services/',
       channel: '#jenkins-pipeline-demo',
       color: 'good', 
       message: 'Welcome to Jenkins, Slack!', 
       teamDomain: 'javahomecloud',
       tokenCredentialId: 'slack-demo'//
   }
}


