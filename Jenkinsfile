node{
	stage('SCM Checkout'){
		git 'https://github.com/epicdominic/rcbcpipeline'
	}
	stage('Compile-Package'){
	sh 'mvn package'
	}
}
