pipeline {

agent any

stages {
         stage('SCM') {
	   steps{
		echo "Code download from Github ..."
	    }
	}
	   stage('Build') {
	      steps {
		echo 'maven build the code ...'
	     }
	}

	  stage('Deploy') {
	     steps{
		echo 'Testing complete & deploy'
	    }
	}
   }

}
