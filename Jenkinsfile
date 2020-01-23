pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
                sh 'mvn clean package spring-boot:repackage'
                sh 'printenv' 
                sh 'java -jar /var/lib/jenkins/workspace/Jenkins_demo/target/demo-0.0.1-SNAPSHOT.jar &'
            }
        }
    }
}
