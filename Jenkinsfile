
node{
	stage('SCM Checkout'){
		git 'https://github.com/saroja-parida/my-app1'
	}
	stage('Compile-Package'){
	def mvnHome = tool name: 'maven-3', type: 'maven'
		sh "${mvnHome}/bin/mvn package"
	}
	stage('email'){
		mail bcc: '', body: '''<html>
               <b>
               This is test email
               </b>
              </html>''', cc: '', from: '', replyTo: '', subject: 'email from jenkin server', to: 'sarojakumarp@gmail.com'
	}
}
