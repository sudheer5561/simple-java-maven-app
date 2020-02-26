pipeline{
    agent any

    choice(name: 'CHOICE', choices: ['master' 'feature'], description 'Pick the branch name you want to deploy' )

    environment{
        PATH = "/opt/apache-maven-3.6.3/bin:$PATH"
    }

    stages{
        
        stage('Checkout'){
            steps{
                git 'https://github.com/sudheer5561/simple-java-maven-app.git'
            }
        }

        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }

    }



}


