pipeline {
agent any
// Get the Maven tool.
// NOTE: This Maven tool must be configured
// in the global configuration.
tools{
maven 'maven-3.6.3'
}
stages{
stage('Build Code'){
	steps{
		bat 'mvn -f maven-demo/pom.xml clean install'
}
	}

	
stage('Run Tests') {
steps {
bat'mvn -f maven-demo/pom.xml test'
}
}
}
}