pipeline{
    agent any
    stages {
        stage('Build App'){
            steps{
                sh "rm -rf SpringBootHelloWorld"
                sh "git clone https://github.com/hugo01718/SpringBootHelloWorld.git/"
                sh "mvn clean -f SpringBootHelloWorld"
                sh "mvn package -f SpringBootHelloWorld"
		sh "sudo mvn install dockerfile:build"
            }
        }
        stage('Deploy DEV'){
            steps{
                sh "ls"
            }
        }
        stage('Promote to UAT'){
            steps{
                sh "ls"
            }
        }
        stage('Deploy UAT'){
            steps{
                sh "ls"
            }
        }
    }   
}
