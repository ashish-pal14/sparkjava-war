pipeline{
	agent any
	environment{
		PATH="/opt/maven/bin:$PATH"
	}
	stages{
		stage('CLONEREPO'){
			steps{
				git url : 'https://github.com/ashish-pal14/sparkjava-war.git' , branch: 'main'
			}
		}
		stage('build'){
			steps{
				sh 'mvn clean install'
			}
		}
	}
}
