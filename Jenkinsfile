pipeline{
    agent any
    stages {
        stage('Build'){
            steps{
                sh 'export BUILD_ID=dontKillMe'
                sh 'source /etc/profile'
                
           
                 withEnv(['JENKINS_NODE_COOKIE=dontkillme']) {
                        sh """
                             nohup java -Dhudson.util.ProcessTree.disable=true -jar /var/lib/jenkins/workspace/Jenkins_demo/target/demo-0.0.1-SNAPSHOT.jar > output 2>&1 &
                        """
                 }
            }
        }
    }
}
