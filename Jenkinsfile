pipeline {
  agent {
      label 'maven' 
  }
	stages{
	  stage ('Build'){
	    steps{
		sh '''
			mvn clean install
			'''
		}
	  }
	  stage ('Unit Test'){
	    steps{
		  jacoco()
		}
	  }
	  stage('testing'){
	    steps{
		  echo "stephie mercy-testing "
		}
		}
      stage('Producton'){
	    steps{
		  echo "This is Prd"
		  } 
		  }
	}
}
