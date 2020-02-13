pipeline {
	agent any
	stages{
		stage('build')
		{
			steps{
				echo 'Project autodeployment is started'
				sh './gradlew build --no-daemon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		stage('Deploytostaging') 
			{
				when {
			      branch 'master'
				}
			      steps
			      {
				  echo 'Projectdelopyment'
			      }
				  
		      }
			      
			      
		           
				   
		       }
		      
		}
	}
}
