pipeline {
    agent any

    stages {
        stage('Set Permissions') {
            steps {
                script {
                    sh """
                    chown -R jenkins:jenkins /var/jenkins_home/workspace/learn-jenkins-app
                    chmod -R 755 /var/jenkins_home/workspace/learn-jenkins-app
                    """
                }
            }
        stage('Git Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}