 pipeline{
     agent any
     stages{
         stage("Build"){
             steps{
                mvn install
                ls
             }
         
        }

    stage("Docker image"){
             steps{
                docker build -t rsvadivu/spring-website:v2 .
             }
         
        }
    stage("Docker push"){
             steps{
                docker push rsvadivu/spring-website:v2 
             }
         
        }
     }
 }