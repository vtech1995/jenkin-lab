import jenkins.*
import hudson.*
import hudson.model.*
import jenkins.model.*

node("Test1"){

     stage("scm checkout"){
          checkout scm
     }
     stage("testing"){
         

      Execution()
     }
}

def Execution(){
     stage("aws tests"){
     withAWS(credentials:'env.Dev',region:'us-west-1') {
       
     }
 }
}       
