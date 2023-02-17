pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				sh 'g++ -o PES2UG20CS375-1 ./new.cpp'
				echo 'Successful building'
			}
		}
		stage('Test'){
			steps{
				sh './PES2UG20CS375-1'
				echo 'Successful testing'
			}
		}
		stage('Deploy'){
			steps{
				echo 'Successful deployment'
			}
		}
	}
	post{
		failure{
			echo 'Pipeline failed'
		}
	}
}
