pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
             
                sh 'nohup java -jar /var/lib/jenkins/workspace/Jenkins_demo/target/demo-0.0.1-SNAPSHOT.jar &'
            }
        }
    }
}
