pipeline {
 agent any
	 stages {
		 stage('Build') {
		 steps {
			 s 'g++ -o PES2UG20CS390-1 ./new.cpp'
			 echo 'BuildiNG successful'
		 }
	 	}
		 stage('Test') {
			 steps {
			 sh './PES2UG20CS390-1'
			 echo 'Testing successful'
			 }
		 }
		 stage('Deploy') {
			 steps {
			 echo 'Deploying successful'
			 }
		 }
	}
	post {
		failure {
		 	echo 'Pipeline failed'
		 }
	 }
}