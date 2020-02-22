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
	 stage ('deployment stage'){
       
	   steps{
	deploy adapters: [tomcat9(path: '', url: '')], contextPath: 'sample123', war: 'C:\\Users\\Toji\\Downloads\\apache-tomcat-9.0.31-windows-x64 (1)\\apache-tomcat-9.0.31\\webapps'
	}
	}
	}
 }
}
	
