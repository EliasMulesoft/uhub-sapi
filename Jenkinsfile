pipeline {
  agent any
  
  stages {
     stage('Build') {
       steps {
         bat 'mvn -B -U -e -V clean -DskipTests package'
  }
  }
     stage('Test') {
       steps {
          echo "******************** MUNIT test execution goes here ***************"
  }
  }
     stage('Deploy Development') {
      steps {
        bat 'mvn -U -V -e -B -DskipTests deploy -Pdev -DmuleDeploy -Dusername=MuleElias5 -Dpassword=Elias885162 -Denc.key=Elias88516280740 -Danypoint.platform.client_id=f10738e6551d447fa369cf2b2cd61806 -Danypoint.platform.client_secret=76E633184Ed44A57Be896516f7a75BB7 -Dbusiness.group=UHO'
  }
  }
  }
  }