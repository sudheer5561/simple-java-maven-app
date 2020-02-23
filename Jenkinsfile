pipepline{
agent any
    stages{
        stage('Checkout code from GIT repository') {
            steps{
                git 'https://github.com/sudheer5561/simple-java-maven-app'
            }
               
        stage('Compile and Build the code') {
            steps{
                sh 'mvn clean package'           
            
            }
               
        }
    }
}



   
