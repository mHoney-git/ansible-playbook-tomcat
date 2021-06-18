pipeline {
    agent any 
    stages {
        stage ('installing tomcat on tomcat-server') {
            steps {
                ansiblePlaybook credentialsId: 'TOMCAT-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'tomcathost.inv', playbook: 'tomcat.yml'
              }
        }
    }
}