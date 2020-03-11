node {

   stage('SCM') {
      // git clone
	  git 'https://github.com/ramesh1239/spring-petclinic.git'
   }
   
   stage ('build the packages') {
      // mvn package
      def mvn_home = tool name: 'maven-3', type: 'maven'
	  sh "${mvn_home}/bin/mvn package"
   }
}
