pipeline{
 agent any
 
 stages{
 stage ('compile stage'){
       
	   steps{
	withMaven(maven : 'apache-maven-3.6.2'){
	        sh 'mvn clean compile'
	}
	}
	}
	stage ('Testing stage'){
       
	   steps{
	withMaven(maven : 'apache-maven-3.6.2'){
	        sh 'mvn test'
	}
	}
	}
	stage ('Deploymenet stage'){
       
	   steps{
	withMaven(maven : 'apache-maven-3.6.2'){
	        sh 'mvn Deploy'
	}
	}
	}
	}
	}
