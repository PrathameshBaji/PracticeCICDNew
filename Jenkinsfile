pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
          
 
          echo  "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
          echo  'git repository name is :' + repository_name
          
           echo "$url$repository_name$ext"
           
          // echo  'git Clone url  is : https://github.com/$owner/$repository_name.git'
           
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
