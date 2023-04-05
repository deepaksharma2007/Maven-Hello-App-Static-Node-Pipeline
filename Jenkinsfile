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
	        sh 'mvn clean package'
		echo 'maven build the code ...'
	     }
	}

	  stage('Test') {
	     steps{
		echo 'Testing complete & deploy'
	    }
	}
	stage('Deploy to Prod'){
	  steps {
	       sh 'java -jar target/*.jar'
	       echo 'Successfully code deployed...'
	      }
   }
  	stage('Archieve'){
	   steps {
	   archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
	   }
}
}
}
