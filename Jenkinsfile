pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
           echo "build success"
      }
    }
    stage('Test') {
      steps {
          echo "mvn test starts"
      }
    }
    stage('Deploy Development') {
      steps {
            bat "mvn clean package deploy -DmuleDeploy -DskipTests -DmuleVersion=4.4.0 -Dusername=rishikasuri2701 -Dpassword=Comicoctober@21 -DapplicationName=exp-bookmyshow-api	 -Denvironment=Sandbox -Dworkers=1 -DworkerType=Micro -DmuleDeploy"
            echo "deploy success"
	  }
	}
  }
}