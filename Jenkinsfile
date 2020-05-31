#!/usr/bin/env grrovy

def myvar1 = "https://github.com"
def myvar2 = ".git"


pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
           
          echo "Hi Prathamesh ..."
          echo "${myvar1}"
          echo "${myvar2}"
           
           script{
              echo "Hi Prathamesh ..."
              echo "${myvar1}"
              echo "${myvar2}"
              echo  'git repository name is :' + repository_name
              echo "$url$repository_name$ext"
              echo "${myvar1}$repository_name$${myvar2}"
           }
           
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
