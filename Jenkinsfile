pipeline{
    agent any
    tools{
        maven 'Maven-New'
    }
    stages{
        stage("Codgite-Checkout")
        {
            steps{
                echo "========executing checkout========"
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        stage("Code-compiling"){
            steps{
                echo "========executing compliation========"
                sh 'mvn compile'
            }
        }
        stage("Test-Code"){
            steps{
                echo "====Code test using surefire===="
                sh 'mvn test'
            }
            
           }
           stage("Build code"){
            steps{
                echo "====building code"
                sh 'mvn package'
            }
           }
    }
    //jenkinsfilepushafterjenkinsjobcreation
    
}

