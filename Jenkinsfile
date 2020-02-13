pipeline {
	agent any
	stages{
		stage('Build')
		{
			steps{
				echo 'Project autodeployment is started'
				sh './gradlew build --no-daemon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
