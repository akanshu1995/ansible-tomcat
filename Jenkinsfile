pipeline{
	agent{ label 'slave1'}
	stages{
	    stage('Tomcat deployment'){
	       steps{
	          script{
              echo "Running playbook"
              ansiblePlaybook colorized: true, credentialsId: '127049a5-3c28-4b6e-b25e-87cff60318a5', inventory: 'inventory', playbook: 'deploy.yml'
            }
        }
	}
}
}
