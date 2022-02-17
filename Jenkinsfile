pipeline {
	agent any
		stages{
	stage('Build') {
		steps{
		echo "Build"
		}
	}
	stage('Test') {
				steps{
		echo "Test"
		}
	}
	stage('Integration Test') {
				steps{
		echo "Int test"
		}
	}
	}

	post{
		always{
			echo "I am succesful"
		}

		success{
			echo "I succeed."
		}
		failure{
			excho "I fail"
		}
	}
}
