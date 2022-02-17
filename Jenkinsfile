pipeline {
	agent { 		
		docker{
			image 'maven:3.6.3'	
		}
	} 
		stages{
	stage('Build') {
		steps{
			sh 'mvn --version'
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
