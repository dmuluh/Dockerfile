pipeline {
   agent any
   stages {
      stage('clone') {
                 steps {
                     sh "git clone https://github.com/dmuluh/Dockerfile.git"
                 }
       }
       stage('build') {
                 steps {
                     sh "docker build -t my-job ."
    
     
                 }
       }
       stage('test') {
                 steps {
                     sh "docker run -itd --name my-jenkinfile-job -p 8081:80 my-job /bin/bash"
    
     
                 }
       }
   }  
}     
