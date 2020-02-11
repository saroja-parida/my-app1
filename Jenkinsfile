
node{
	stage('SCM Checkout'){
		git 'https://github.com/saroja-parida/my-app1'
	}
	stage('Compile-Package'){
	sh 'mvn package'
	}
}
