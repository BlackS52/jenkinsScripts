#Jenkinsfile (Declarative Pipeline)
pipeline {
	agent { 
		node { label 'gnomeOverlord' }
	}

	parameters {
    	booleanParam(defaultValue: true, description: 'Build OMPI', name: 'BUILD')
    	booleanParam(defaultValue: true, description: 'Deploy OMPI', name: 'DEPLOY')
    	booleanParam(defaultValue: false, description: 'Remove OMPI', name: 'REMOVE')
	}


	environment {
   	SSISBuildPath="/home/mpi_test/jenkins_stuff/ompi/"
		SSISDeployPath="/home/mpi_test/jenkins_stuff/ompi_install"
	}

#	docker { image 'python:3.10.1-alpine' } 
#	}

   stages {
		stage('check') { 
            steps {
               sh 'python --version'
					echo 'Check version'
          }
#		stage('Build') { }
# 		stage('Deploy') { }       
   }
}
