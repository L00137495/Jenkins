pipeline {
agent any
// Get the Maven tool.
// NOTE: This Maven tool must be configured
// in the global configuration.
tools{
maven 'Maven'
}
stages{
stage('Build Code'){
	steps{
		bat 'mvn -f my-app/pom.xml clean install'
}
	}

	
stage('Run Tests') {
steps {
bat 'mvn -f my-app/pom.xml test'
}
}
}
}
