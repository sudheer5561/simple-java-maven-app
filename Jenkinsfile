pipeline{

    agent any

/* Declarative Directive Generator */

    parameters { choice choices: ['Master', 'feature1', 'feature2'], description: '', name: 'BuildName' }

    environment{

        PATH = "/opt/apache-maven-3.6.3/bin:$PATH"

            }

    stages{

        stage('GIT Checkout'){
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
