pipeline {
  agent any  
  stages{
    stage('clone'){
steps{
 echo "first step"
}
}
stage('SonarQube Scan'){
 steps{
   echo "2 step"
 }
}  
    stage('Unit Test'){
 steps{
   echo "3 step"
 }
}  
stage('Build War'){
 steps{
   echo "4 step"
 }
    }  
stage('Upload War'){
 steps{
   echo "5 step"
 }
}

stage('Deploy War'){
 steps{  
git branch: 'master',
credentialsId:'63728019-0db2-4d89-85f5-5b182130ea55',
url:'git@github.com:sharathgoud2016/DemoAppSample.git'
 }       
     
 }  
stage('Send Email'){
 steps{
   mail bcc: '', body: 'Pipeline', cc: 'mohanraj123@gmail.com', from: '', replyTo: '', subject: 'From Sharath', to: 'sharathgoud2016@gmail.com'
 }  
    }
 }
}
