pipeline {
 agent any
	 stages {
		 stage('Build') {
		 steps {
			 s 'g++ -o PES2UG20CS375-1 ./main/hello.cpp'
			 echo 'Successful building'
		 }
	 	}
		 stage('Test') {
			 steps {
			 sh './PES2UG20CS375-1'
			 echo 'Successful testing'
			 }
		 }
		 stage('Deploy') {
			 steps {
			 echo 'Successful deployment'
			 }
		 }
	}
	post {
		failure {
		 	echo 'Pipeline failed'
		 }
	 }
}