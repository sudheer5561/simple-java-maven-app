pipeline{
    agent any
        stages{
            stage('SCM GIT Checkout') {
                steps{
                git 'https://github.com/sudheer5561/simple-java-maven-app'
                }
            }
            stage('compile and build') {
                steps{
                sh 'mvn clean package'
                }
            }
        }
}
