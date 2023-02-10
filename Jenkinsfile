pipeline{
    agent any
    stages{
        stage ('SCM Checkout'){
            steps {
                git "https://github.com/Narasimha8780/shan-ansible.git"
            }
        }
        stage('Execute Ansible'){
            steps{
                ansiblePlaybook credentialsId: 'ubuntu', inventory: 'dev.inv', playbook: 'apache.yml'
                }
        }
            
    }    
}
