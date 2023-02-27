node('nodes'){
    
 def mavenHome = tool name: "maven-3.8.2"    
    
 stage('CheckOutCode')
 {
 git branch: 'development', credentialsId: 'e108d759-8776-4f2e-ac2b-09f07558548c', url: 'https://github.com/punu765/maven-web-application.git'
 }
 
 stage('Build')
 {
   sh "${mavenHome}/bin/mvn clean package"
 }
 /*
 stage('SonarQubeReport')
 {
   sh "${mavenHome}/bin/mvn clean sonar:sonar"
 }
 
 stage('UploadArtifactIntoNexus')
 {
   sh "${mavenHome}/bin/mvn clean deploy"
 }
 
 stage('DeployAppIntoTomcatServer')
 {
   sshagent(['368819a0-909b-4bd3-86f8-77f1cf83865d']) {
    sh "scp -o StrictHostKeyChecking=no  target/maven-web-application.war ec2-user@15.206.173.183:/opt/apache-tomcat-9.0.71/webapps/"
 }
 }
 
 stage('SendEmailNotification')
 {
   emailext body: '''Build is over

regards
puneeth''', subject: 'Build Over', to: 'puneeth.bh02@gmail.com'
 }
 
 */
 }

