pipeline{
    
    agent any
    
    stages{
        stage('Checkout'){
            steps{
                git(url: 'https://github.com/Yash-Repalle/Java_App', branch: 'main')
            }
        }
        
        stage('Test'){
            steps{
                 sh 'mvn test'
            }
        }
        
        stage('Intigration Test'){
            steps{
                 sh 'mvn verify -DskipUnitTests'
            }
        }
    }
}
