pipeline{
 agent any
 
 stages{
 stage ('compile stage'){
       
	   steps{
	withMaven(maven : 'apache-maven-3.6.2'){
	        bat 'mvn verify'
	}
	}
	}
	 stage ('Testing stage'){
       
	   steps{
	withMaven(maven : 'apache-maven-3.6.2'){
	        bat 'mvn test'
	}
	}
	}
	
	
	}
 }
