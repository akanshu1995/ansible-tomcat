pipeline{
	agent{ label 'slave1'}
	stages{
	    stage('Tomcat deployment'){
	       steps{
	          script{
              echo "Running playbook"
              ansiblePlaybook colorized: true, credentialsId: 'ansible-id', inventory: 'inventory', playbook: 'deploy.yml'
            }
        }
	}
}
}
