import jenkins.*
import hudson.*
import hudson.model.*
import jenkins.model.*

node("Test1"){

     
     stage("testing"){
         

      Execution()
     }
}

def Execution(){
     stage("aws tests"){}
     withAWS(credentials:'env.Dev',region:'us-west-1') {
       //cfnDeploy(file:'ec2.yml', stackName:"Jenkins-ec2")
       def response = cfnValidate(file:'ec2.yaml')
       echo "template description: ${response.description}"
}
        
