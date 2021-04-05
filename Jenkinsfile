pipeline {
   agent any
   environment {
       BranchName="master"
   }
   stages {
      stage('Start build') {
         steps {
            echo 'Start build'
            //sleep 360
            //sleep 15
            //dir('/var/jenkins_home/workspace') {
               //sh 'ps'
            //}
            echo 'Build runing'
            //sh "pwd"
         }
      }
      stage('Code review'){
         steps {
           echo "This is Codeing......"
           //sleep 30
           sh "pwd"
           echo "runing master"
           sh "ps -a"
         }
      }
      stage('Test runing'){
         when {
            branch 'master'
         }
         steps {
           //sleep 15
           echo "runing master"
         }
      }
      stage('Deploy ending') {
         environment {Description="This is "}
         steps{
            script{
               if (env.GIT_BRANCH == 'origin/F2048'){
                  echo "${Description}${BranchName}"
                  //sleep 25
                  sh "ls"
               }
            }
         }
      }
   }
}
