pipeline{

 agent {
 label "Redmine"
   }

 stages{

   stage("Build"){

     steps{

      sh "cd /var/lib/jenkins/redmine/jobs ; mkdir  ${env.BUILD_NUMBER} ; cd ${env.BUILD_NUMBER} git clone git@github.com:Mohab-eSpace/Redmine-test.git"

      sh "cd /var/lib/jenkins/redmine  ; ln -s jobs/${env.BUILD_NUMBER} public"


    }
  }
 }
}
