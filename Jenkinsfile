node {
    withMaven(maven:'maven') {
        stage('Checkout') {
            git 'https://github.com/epicdominic/rcbcpipeline'
        }
        stage('Build') {
            sh 'mvn clean install'
            def pom = readMavenPom file:'pom.xml'
            print pom.version
            env.version = pom.version
	}
    }
}
