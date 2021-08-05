node{

stage('CheckoutCode'){
 git branch: 'development', credentialsId: 'bc24a5fc-5bfc-49fd-8240-82695e50796f', url: 'https://github.com/sreedhark9/maven-web-application.git'
}

stage('Build'){
sh "mvn clean package"
}

/*
stage('ExcuteSonarQubeReport'){
sh "${mavenHome}/bin/mvn sonar:sonar"
}

stage('UploadArtifactIntoNexus'){
sh "${mavenHome}/bin/mvn deploy"
}

stage('DeployAppIntoTomacatServer')
{
sshagent(['0b8828ef-8dcc-4894-bf3b-40d8ae32d353']) {
 sh"scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@13.233.153.185:/opt/apache-tomcat-9.0.50/webapps/"
}
{

stage("SendEmailNotification")
{
emailext body: '''build over 
regards,
sreedhar''', subject: 'build over ', to: 'vijayvijay205@gmail.com'
}
*/

}

