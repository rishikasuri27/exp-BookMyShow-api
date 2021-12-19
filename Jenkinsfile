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
            bat "mvn clean package deploy -DmuleDeploy -DskipTests -DmuleVersion=4.4.0 -Dusername=rishikasuri2701 -Dpassword=Comicoctober@21 -DapplicationName=exp-bookmyshow-api -Denvironment=Sandbox -Dworkers=1 -DworkerType=Micro -DmuleDeploy -Danypoint.platform.client_id=a7e5bde4364741a98577b41acc43dc8f -Danypoint.platform.client_secret=28e68C2156724690B244c283BEfe361a"
            echo "deploy success"
	  }
	}
  }
}