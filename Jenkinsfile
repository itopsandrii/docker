pipeline {
  agent  {
       label 'jenkins_slave'
  }
  
  stages {
     stage('build') {
	    steps {
		           echo 'genetating file 100MB'
		           sh 'fallocate -l 100MB test.txt'
		}	   
	 }
    stage('testing') {
	    steps {
	                  echo 'arcive file'
		          sh 'gzip test.txt'
		          echo 'file size'
		          sh 'ls -lh'
	    }
     }
  }	  
}
