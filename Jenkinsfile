def workSpace;
node {
   stage ("CheckOut"){
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '205fc29d-5aea-449d-bcd0-76678991eb04', url: 'https://github.com/akash-jasani/git_repo.git']]])
       workSpace = /home/vagrant/
   }
   stage ("Static Code Analysis ") {
       echo "Static Code analysis"
   }
   stage ("Build"){
       echo "Generate Build"
   }
   stage ("Unit Test"){
       echo "Unit Test"
   }
   stage ("Delivery"){
       echo "Deliver to the production"
   }
}
