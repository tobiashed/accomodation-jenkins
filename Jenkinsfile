pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                checkout scm
            
            }
          
        }
        stage('Build web-app'){
            steps{
                sh 'mvn -f /home/robot/.jenkins/workspace/test-jenkins-pipeline/hoteljsf clean install'
            
            }
          
        }
        stage('Build web-service'){
            steps{
                sh 'mvn -f /home/robot/.jenkins/workspace/test-jenkins-pipeline/hotel-restfull clean install'
            
            }
          
        }
    }

}
