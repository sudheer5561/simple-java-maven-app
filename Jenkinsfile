pipeline{
    agent any

    choice(name: 'CHOICE', choices: ['master' 'feature'], description 'Pick the branch name you want to deploy' )

    stages{
        
        stage('Checkout'){
            steps{
                git 'https://github.com/sudheer5561/assignment.git'
            }
        }

        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }

    }



}
