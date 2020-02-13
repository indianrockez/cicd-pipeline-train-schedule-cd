pipeline {
	agent any
	stages{
		stage('build')
		{
			steps{
				echo 'Project autodeployment is started'
				sh './gradlew build --no-daemon'
				archiveArtifacts artifacts: 'dist/trainschedule.zip'
			}
		}
	}
}
