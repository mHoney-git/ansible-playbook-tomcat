pipeline {
    agent any 
    stages {
        // stage ('installing apache on apache-web server') {
        //     steps {
        //         ansiblePlaybook credentialsId: 'AWS-SSH-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'apache.yml'
        //       }
        // }

        stage ('installing tomcat on tomcat-server') {
            steps {
                ansiblePlaybook credentialsId: 'TOMCAT-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'tomcathost.inv', playbook: 'tomcat.yml'
              }
        }

        // stage ('installing Jboss on Jboss-server') {
        //     steps {
        //         ansiblePlaybook credentialsId: 'JBOSS-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'Jbosshosts.inv', playbook: 'Jboss.yml'
        //       }
        // }

    }
}