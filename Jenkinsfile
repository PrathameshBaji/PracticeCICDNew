pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
  //        def command = "basename -s .git 'git config --get remote.origin.url' "

   //      def proc = command.execute()
   //      proc.waitFor()              

   //      if ( proc.exitValue() != 0 ) {
   //         println "Error, ${proc.err.text}"
   //         System.exit(-1)
   //      }

   //      def branches = proc.in.text.readLines().collect { 
   //          it.replaceAll(/[a-z0-9]*\trefs\/heads\//, '') 
    //     }

//println branches
          echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
           echo $.repository.clone_url
        }
   }
   stage('Test') {
     steps {
        echo 'Testing...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying...'
     }
   }
  }
}
