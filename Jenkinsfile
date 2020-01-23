pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
                sh 'cd /var/lib/jenkins/workspace/Jenkins_demo/target/'
                sh 'nohup java -jar demo-0.0.1-SNAPSHOT.jar &'
            }
        }
    }
}
